<template>
    <div>
        <h1>form validation</h1>
        <input type="text" v-model="loginform.username" name="user" placeholder="Enter user id"/>
        <br>
        <input type="password" v-model="loginform.password"  name="password" placeholder="enter password"/>
        <br>
        <button v-on:click="logindata">login</button>
    </div>
</template>
<script>
export default {
    name:"login",
    methods:{
        logindata(){
            console.log(this.loginform.username,this.loginform.password)

        }
        
        },
    data(){
        return {loginform:{
            username:null,
            password:null,
        }}
    }
}
</script>