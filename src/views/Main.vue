<template>

    <el-container style="height:100%">
        <el-aside width="auto">
            <CommonAsideVue></CommonAsideVue>
        </el-aside>
        <el-container>
            
            <el-header>
                <CommonHeaderVue></CommonHeaderVue>
            </el-header>

            <CommonTagVue></CommonTagVue>

            <el-main>
                <router-view></router-view>
            </el-main>
            
        </el-container>


    </el-container>

</template>
<script>
import CommonAsideVue from '@/components/CommonAside.vue';
import CommonHeaderVue from '@/components/CommonHeader.vue';
import CommonTagVue from '@/components/CommonTag.vue';

export default {
    name: "commonMain",
    components:{
        CommonAsideVue,
        CommonHeaderVue,
        CommonTagVue
    },
    data() {
        return {};
    },
};
</script>
<style lang="less" scoped>
.el-header {
    background-color: #333;
}

.el-main {
    padding-top: 0;
}
</style>