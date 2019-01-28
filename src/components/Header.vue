<template>
    <div class="header">
        <el-menu
                background-color="#0C2135"
                text-color="#bfcbd9"
                active-text-color="#409EFF"
                :default-active="$route.path"
                class="el-menu"
                mode="horizontal">
            <el-menu-item index="1">
                <router-link to="/">
                    <div>Home</div>
                </router-link>
            </el-menu-item>
            <el-menu-item index="2">
                <router-link to="/about">
                    <div>About</div>
                </router-link>
            </el-menu-item>
            <el-submenu index="3">
                <template slot="title">我的工作台</template>
                <el-menu-item index="2-1">选项1</el-menu-item>
                <el-menu-item index="2-2">选项2</el-menu-item>
                <el-menu-item index="2-3">选项3</el-menu-item>
                <el-submenu index="2-4">
                    <template slot="title">选项4</template>
                    <el-menu-item index="2-4-1">选项1</el-menu-item>
                    <el-menu-item index="2-4-2">选项2</el-menu-item>
                    <el-menu-item index="2-4-3">选项3</el-menu-item>
                </el-submenu>
            </el-submenu>
            <el-menu-item index="4"><a href="https://www.ele.me" target="_blank">订单管理</a></el-menu-item>
        </el-menu>
    </div>
</template>

<script>
    export default {
        name: "Header"
    }
</script>

<style scoped>

    .header {
        background-color: #0C2135;
    }

    /*去掉导航栏底部白线*/
    .el-menu.el-menu--horizontal {
        border-bottom: 0;
    }

    a {
        text-decoration: none;
    }

</style>
