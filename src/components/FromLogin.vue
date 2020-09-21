<template>
    <div>
        <form>
            login: <br/>
            Email : 
            <input type='email' /> <br/>
            password : <br/>
            <input type='password'/> <br/>
        </form>
    </div>       
</template>

<script>
export default {
    data() {
        return{
        email: '', 
        password: '', 

        }
    }
}
</script>