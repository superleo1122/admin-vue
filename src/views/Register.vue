<template>
    <div class="register_container">
        <div class="register_box">
            <h1>Hello World</h1>

        </div>
    </div>
</template>

<script lang="ts">
    import { Component,Vue } from 'vue-property-decorator'

    @Component({
        name:'Register'
    })
    export default class Register extends Vue{

    }
</script>

<style lang="scss" scoped>
    .register_container{
        width: 100%;
        height: 100%;
        background-color: red;
        .register_box{
            width: 500px;
            height: 300px;
            background: #cccccc;
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