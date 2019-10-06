<template>
    <header v-vue-scrollup-menu class="header">
        <h1>
            <span style='color: orange'>h</span>
            <span style='color: pink'>o</span>
            <span style='color: yellow'>m</span>
            <span style='color: blue'>e</span>
        </h1>
    </header>
</template>

<script>
    import vueScrollupMenu from 'vue-scrollup-menu'

    export default {
        name: "SemiStickyHeader",
        directives: {
            vueScrollupMenu
        },
        components: {
        }
    }
</script>

<style lang="scss" scoped>
    .header {
        -webkit-box-shadow: 0 3px 5px rgba(57, 63, 72, 0.3);
        -moz-box-shadow: 0 3px 5px rgba(57, 63, 72, 0.3);
        box-shadow: 0 3px 5px rgba(57, 63, 72, 0.3);
        font-size:24px;
        width:100%;
        height:100px;
        background:white;
        position:fixed;
        text-align: center;
        line-height: 50px;
        top: 0;
        left: 0;
        img {
            max-height: 120%;
            left: 0;
        }
        h1 {
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: -6px;
            line-height: 50px;
            float: left;
            padding-left: 30px;
        }
        nav {
            float: right;
            padding-right: 35px;
            line-height: 50px;
            ul li {
                list-style: none;
                display: inline-block;
                margin-left: 25px;
                a {
                    text-decoration: none;
                    color: #767d88;
                    &:hover {
                        color: #f67600;
                    }
                }
            }
        }
    }

</style>
