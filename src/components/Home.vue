<template>
<h1>Simple form</h1>
<p>
    {{ form }}
</p>
<form>
    <label>Email</label>
    <input type="text" placeholder="Enter Email" v-model="form.email" />
    <br />
    <br />
    <label>Password</label>
    <input type="password" placeholder="Enter Password" v-model="form.password" />
    <br />
    <br />
    <select v-model="form.country">
        <option>India</option>
        <option>US</option>
        <option>China</option>
    </select>
    <br />
    <br />
    <h3>Technology</h3>
    <label>Html</label>
    <input type="checkbox" value="html" v-model="form.technology" />
    <br />
    <br />
    <label>Java</label>

    <input type="checkbox" value="java" v-model="form.technology" />
    <br />
    <br />
    <h3>Gender</h3>
    <label>Male</label>

    <input type="radio" value="male" name="gender" v-model="form.gender" />
    <label>Female</label>

    <input type="radio" value="female" name="gender" v-model="form.gender" />

    <button type="button" v-on:click="login">Click Me</button>
</form>
</template>

<script>
export default {
    name: 'HomeComp',
    data() {
        return {
            form: {
                email: '',
                password: '',
                country: '',
                technology: [],
                gender: ''
            }
        }
    },
    methods: {
        login() {
            console.warn("login data", this.form)
        }
    }

}
</script>

<style scoped>
h1 {
    color: red
}
</style>
