<template>
    <div class="title flex-centured " :class="{checked: tarefa.checked}">
         <dir class="title-content">
            <div class="title-subtitle"> {{tarefa.description}}</div>
            <div>{{tarefa.checked}}</div>
         </dir>

         <div class="title-action">
            <button @click="$emit('toggle', tarefa)" class="btn btn-primary">
                <span v-if="tarefa.checked"> Desmarcar</span>
                <span v-else>Concluido</span>
            </button>
            <button  @click="$emit('remove',tarefa)" class="btn btn-error"> Remover</button>
         </div>
         
    </div>
</template>
<script>


    export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Tarefa",
    props: {
            tarefa: {type: Object, required: true}
    }
};

</script>
<style scoped>
    .checked {
        text-decoration: line-through;
        color: lightslategray;
    }
</style>