<template>
    <div id="app">
        <div>
            <el-row>
                <el-col :span="24">
                    <Header/>
                </el-col>
            </el-row>
            <el-row>
                <el-col :span="24">
                    <router-view/>
                </el-col>
            </el-row>
            <el-row>
                <el-col :span="24">
                    <Footer/>
                </el-col>
            </el-row>
        </div>
    </div>
</template>

<script>
    import Header from './components/Header'
    import Footer from './components/Footer'

    export default {
        components: {Header, Footer}
    }
</script>

<style>
    #app {
        font-family: "Helvetica Neue", Helvetica, "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", "微软雅黑", Arial, sans-serif;
        /*-webkit-font-smoothing: antialiased;*/
        /*-moz-osx-font-smoothing: grayscale;*/
        text-align: center;
        /*color: #2c3e50;*/
    }
</style>
