<template>
    <div>
        <form @submit.prevent="handleSubmit">
            login: <br/>
            Email : 
            <input type='email' v-model="email" /> <br/>
            password : <br/>
            <input type='password' v-model="password"/> <br/>

            <button type="submit">login now</button>
        </form>   
    <div>
        <p>
            Email: {{ email }} <br/>
            Password: {{ password }}
        </p>    
    </div>
    </div>
</template>

<script>
export default {
    data() {
        return{
        email: 'coucou@gmail.com', 
        password: 'paswword', 

        }
    },

    methods: {
        handleSubmit (){
            alert('login ?', this.email, this.password )
        }
    }
}
</script>