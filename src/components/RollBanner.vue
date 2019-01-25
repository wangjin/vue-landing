<template>
    <el-carousel height="650px">
        <el-carousel-item>
            <img src="https://zos.alipayobjects.com/rmsportal/xHxWkcvaIcuAdQl.jpg" />
        </el-carousel-item>
        <el-carousel-item>
            <img src="https://zos.alipayobjects.com/rmsportal/hzPBTkqtFpLlWCi.jpg" />
        </el-carousel-item>
    </el-carousel>
</template>

<script>
export default {
    name: 'RollBanner'
}
</script>

<style scoped>
    .el-carousel__item h3 {
        color: #475669;
        font-size: 14px;
        opacity: 0.75;
        line-height: 150px;
        margin: 0;
    }

    .el-carousel__item:nth-child(2n) {
        background-color: #99a9bf;
    }

    .el-carousel__item:nth-child(2n+1) {
        background-color: #d3dce6;
    }
</style>
