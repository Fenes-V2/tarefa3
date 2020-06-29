<template>
    <div id="adicionar">
        <input type="text" placeholder="Insira uma tarefa" class="adicionado" v-model="informacao" />
        <button @click="processar">Enviar</button>
    </div>
</template>

<script>
export default {
    name: "novo",
    data: function() {
        return {
            informacao: ""
        };
    },
    methods: {
        processar: function() {
            this.$store.commit("processar", {
                informacao: this.informacao
            });
        }
    }
};
</script>

<style>
</style>