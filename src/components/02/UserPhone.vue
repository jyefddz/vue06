<template>
    <div>
        <div>
            <p style="color:#ccc">选择所在地区(实名认证主体所在地)</p>
            <input type="radio" name="area" id="中国大陆">中国大陆
            <input type="radio" name="area" id="中国香港">中国香港
        </div>
        <div style="margin-bottom:10px">
            <p>手机号码</p>
            <select>
                <option value="1">86</option>
                <option value="2">82</option>
                <option value="3">886</option>
                <option value="4">882</option>
            </select>
            <input type="text" placeholder="请输入手机号码">
        </div>
        <div style="margin-bottom:10px">
            <input type="text" placeholder="请输入验证码"> 
            <button style="background-color:blue;border-radius: 5px;"><span style="color:#fff">发送验证码</span></button>
        </div>
        <div style="margin-bottom:10px">
            <input type="password" placeholder="请输入密码">
        </div>
        <div>
            <input type="password" placeholder="请确认密码">
        </div>
    </div>
</template>

<script>
export default {
}

</script>

<style>
</style>