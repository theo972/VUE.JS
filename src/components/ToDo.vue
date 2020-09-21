<template>
    <div>
        <form @submit.prevent="SubmitText">
            <input type='text' v-model="text" /> <br/>
            <button type ="submit">Valider</button>
        </form>
        <div>
            <div v-for="(item, index) in tableau" :key="index">   
                <input type ="checkbox">
                {{ item }}

            </div>
        </div>
    </div>
    

</template>

<script>
export default {
    data(){
        return{
            tableau: ['theo','erot','toertt'],
            text: "",
        }
    },

     methods:{
         SubmitText () {
            this.tableau.push(this.text);


         }
     } 

}
</script>