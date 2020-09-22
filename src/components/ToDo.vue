<template>
    <div>
        <form @submit.prevent="SubmitText">
            <input type='text' v-model="text" /> <br/>
            <button type ="submit">Valider</button>
        </form>
        <div>
            <div v-for="(item, index) in tableau" :key="index">   
                <input type ="checkbox" />
                {{ item }}
  
        {{ item.name }}
                <button @click.stop.prevent="DeleteText(index)">X</button>
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
            checkbox: "",
        }
    },

     methods:{
         SubmitText () {
            this.tableau.push(this.text);


         }
     }, 
        DeleteText (index) {
            this.tableau.splice(index, 1);
        }

}
</script>