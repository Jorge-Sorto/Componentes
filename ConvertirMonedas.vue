<template>
    <div>
        <br>
        <br>
        <h2>Dolares a Euros</h2>
        <input v-model="vEntrada" type="numbre" placeholder="Ingrese la cantidad de dolares"/>
        <br>
        <b-button variant="success" v-on:click="Calcularmoneda" title="Convertir">Convertir</b-button>
        <br>
        <h4>{{vEntrada}} dolares equivalen a: {{resultado}} euros</h4>

    </div>
</template>
<script>
export default{
    name: 'ConvertirMonedas',
    data(){
        return{
            vEntrada: '',
            resultado: ''
        }
    },
    methods:{
        Calcularmoneda(){
            this.resultado = this.vEntrada * 0.88;
            console.log(this.vEntrada);
            console.log(this.resultado)
        }
    }
}
</script>
