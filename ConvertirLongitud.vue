<template>
    <div>
        <br>
        <br>
        <h2>Metros a Centimetros</h2>
        <input v-model="vEntrada" type="numbre" placeholder="Ingrese los metros a convertir"/>
        <br>
        <b-button variant="success" v-on:click="Calcularlongitud" title="Convertir">Convertir</b-button>
        <br>
        <h4>{{vEntrada}} metros equivalen a: {{resultado}} centimetros</h4>

    </div>
</template>
<script>
export default{
    name: 'ConvertirLongitud',
    data(){
        return{
            vEntrada: '',
            resultado: ''
        }
    },
    methods:{
        Calcularlongitud(){
            this.resultado = this.vEntrada * 100;
            console.log(this.vEntrada);
            console.log(this.resultado)
        }
    }
}
</script>
