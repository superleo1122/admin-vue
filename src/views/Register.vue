<template>
    <div class="register_container">
        <div class="register_box">
            <h1>Hello World</h1>
            <el-tabs tab-position="left" style="height: 70%;">
                <el-tab-pane label="普通注册">
                    <NormalForm></NormalForm>
                </el-tab-pane>
                <el-tab-pane label="手机注册">配置管理</el-tab-pane>
                <el-tab-pane label="邮箱注册">角色管理</el-tab-pane>
            </el-tabs>
        </div>
    </div>
</template>

<script lang="ts">
    import { Component,Vue } from 'vue-property-decorator'
    import NormalForm from "@/components/NormalForm.vue";

    @Component({
        name:'Register',
        components:{
            NormalForm
        }
    })
    export default class Register extends Vue{

    }
</script>

<style lang="scss" scoped>
    .register_container{
        width: 100%;
        height: 100%;
        background-color: #cccccc;
        .register_box{
            width: 500px;
            height: 350px;
            padding-left: 10px;
            padding-right: 40px;
            background: #ffffff;
            position: absolute;
            left: 50%;
            top: 50%;
            transform:translate(-50%,-50%);
            border-radius: 10px;
            h1{
                text-align: center;
            }
        }
    }
</style>