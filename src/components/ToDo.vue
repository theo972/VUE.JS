<template>
    <div>
        <form @submit.prevent="deletetodo">
            <select todoli ="todolist" size="1">
            <option>theo</option>
            <option>antho</option>
            <option>Jimmy</option>
            </select>
            <br/>
            <button type="submit">retire de la todolist</button>
        </form>  
        <form @submit.prevent="handleSubmits">
         <br/>
            Rajouter une tache : 
            <input type='text' v-model="text" /> <br/> 
             <button type="submit">Rajouter</button>
        </form>
    <div>
        <p>
            todolist: {{ todoli }} <br/>
            text: {{ text }} 
        </p>    
    </div>
    </div>
</template>

<script>
export default {
    data() {
        return{
            todoli: 'prout', 
            text: '',
        }
    },

    methods: {
        deletetodo (){
            
        },
        handleSubmits (){
            alert('vous avez rajouter' + text )
        }
    }
}

</script>