<template>
    <div class="title flex-centured " :class="{checked: tarefa.checked}">
         <dir class="title-content">
            <div class="title-subtitle"> {{tarefa.description}}</div>
         </dir>

         <div class="title-action">
            <button @click="$emit('toggle', tarefa)" class="btn title-primary"> CONCLUIDO</button>
            <button class="btn title-erro"> REMOVER</button>
         </div>
         
    </div>
</template>
<script>


    export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Tarefa",
    props: {
        tarefa: {
            tarefa: {type: Object, required: true}
        }
    }
    
}

</script>
<style scoped>

</style>