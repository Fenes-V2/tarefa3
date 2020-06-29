<template>
    <div id="app">
        <novo/>
        <coisas/>
    </div>
</template>

<script>
import coisas from "./components/coisas.vue"
import novo from "./components/novo.vue"
export default {
    name: "App",
    components: {
        coisas,
        novo
    }
};
</script>

<style>
#tarefasio {
    width: 380px;
    height: 300px;
    border: 3px solid #ffffff;
    margin: 1px auto 0px auto;
    user-select: none;
    padding: 10px;
}
#adicionar {
    width: 380px;
    height: 130px;
    border: 3px solid #ffffff;
    margin: 5px auto 0 auto;
    padding: 10px;
}
.adicionado {
    width: 150px;
    text-align: center;
    margin: 50px 10px 10px 90px;
}
</style>
