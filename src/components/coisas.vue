<template>
    <div id="tarefasio">
        <div class="trabalhos" v-for="(afazer, informacao) in tarefas" :key="informacao">
            {{ afazer.informacao }}
            <input type="checkbox" />
        </div>
    </div>
</template>

<script>
export default {
    name: "coisas",
    data: function() {
        return {
            informacao: ""
        };
    },
    computed: {
        tarefas() {
            return this.$store.state.tarefas;
        }
    }
};
</script>

<style>
</style>