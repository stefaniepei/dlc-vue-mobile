<template>
    <div class="page setting">
        <mt-header title="账户设置" class="header-bg-color">
            <router-link to="/info" slot="left">
                <mt-button icon="back"></mt-button>
            </router-link>
        </mt-header>
    
        <div>
            <section class="arrow-line">
                <em>
                    <img src="../../assets/images/account/me.png" />
                </em>
                <span>手机号</span>
                <span class="float-right margin-right-15">{{this.userAccount['cellphone']}}</span>
            </section>
    
            <router-link to="/changePwd/back" class="arrow-line" tag="section">
                <em>
                    <img src="../../assets/images/account/login-pwd.png" />
                </em>
                <span>登录密码</span>
                <span style="float: right;">修改
                    <span class="arrow-right"></span>
                </span>
            </router-link>
    
            <router-link to="/transactionPwd" class="arrow-line" tag="section">
                <em>
                    <img src="../../assets/images/account/login-out.png" />
                </em>
                <span>退出</span>
                <span style="float: right;">退出
                    <span class="arrow-right"></span>
                </span>
            </router-link>
        </div>
    </div>
</template>
<script>
import { mapGetters } from 'vuex'
export default {
    computed: mapGetters([
        'userAccount'
    ]),
}
</script>
<style scoped>

</style>