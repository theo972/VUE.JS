<template>
    <div>
        <form>
            login: <br/>
            Email : 
            <input type='email' /> <br/>
            password : <br/>
            <input type='password'/> <br/>

            <button type="submit">login now</button>
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