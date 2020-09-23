<template>
    <el-form ref="form" :model="registerData" label-width="0px">
        <el-form-item label="">
            <el-input v-model="registerData.username" prefix-icon="el-icon-user" placeholder="账号"></el-input>
        </el-form-item>
        <el-form-item label="">
            <el-input v-model="registerData.password" prefix-icon="el-icon-lock" placeholder="密码"></el-input>
        </el-form-item>
        <el-form-item label="">
            <el-row :gutter="20">
                <el-col :span="14">
                    <el-input v-model="registerData.captcha" prefix-icon="el-icon-lock" placeholder="验证码"></el-input>
                </el-col>
                <el-col :span="6">
                    <img src="../assets/code.png" style="width: 120px; height: 40px">
                </el-col>
            </el-row>
        </el-form-item>
        <el-form-item>
            <el-button type="primary" @click="onSubmit" style="width: 100%">注册</el-button>
        </el-form-item>
    </el-form>
</template>

<script lang="ts">
    import {Vue, Component, Ref} from 'vue-property-decorator'

    @Component({
        name: 'NormalForm',
    })
    export default class NormalForm extends Vue{
        registerData = {
            username: '',
            password: '',
            captcha: '',
            registerType: 'normal',
        }
        onSubmit(){

        }
    }
</script>