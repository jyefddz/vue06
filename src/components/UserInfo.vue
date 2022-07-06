<template>
        <div>
            <button @click="comName = 'UserPhone'" style="border: 0px;background-color: #fff;">手机注册</button>
            <button @click="comName = 'UserEmail'" style="border: 0px;background-color: #fff;">邮箱注册</button>
            <div>
                <keep-alive include="UserPhone">1
                    <component :is="comName"></component>
                </keep-alive>
            </div>
        </div>
</template>

<script>
import UserEmail from './02/UserEmail.vue'
import UserPhone from './02/UserPhone.vue'
export default {
    data() {
        return {
            comName: UserEmail
        }
    },
    components: {
        UserEmail,
        UserPhone
    }
}
</script>

<style>
</style>


