<template>
    <div>
        <h1>Conversor de Unidades de Medida</h1>
        <br>
        <br>
        <h2>Libras a kilogramos</h2>
        <input v-model="vEntrada" type="numbre" placeholder="Ingrese la cantidad en libras"/>
        <br>
        <b-button variant="success" v-on:click="Calcularmasa" title="Convertir">Convertir</b-button>
        <br>
        <h4>{{vEntrada}} libras equivalen a: {{resultado}} kilogramos</h4>

    </div>
</template>
<script>
export default{
    name: 'ConvertirMasa',
    data(){
        return{
            vEntrada: '',
            resultado: ''
        }
    },
    methods:{
        Calcularmasa(){
            this.resultado = this.vEntrada * 0.45;
            console.log(this.vEntrada);
            console.log(this.resultado)
        }
    }
}
</script>
