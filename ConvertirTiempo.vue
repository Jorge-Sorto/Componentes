<template>
    <div>
        <br>
        <br>
        <h2>Minutos a Segundos</h2>
        <input v-model="vEntrada" type="numbre" placeholder="Ingrese el numero de minutos"/>
        <br>
        <b-button variant="success" v-on:click="Calculartiempo" title="Convertir">Convertir</b-button>
        <br>
        <h4>{{vEntrada}} minutos equivalen a: {{resultado}} segundos</h4>

    </div>
</template>
<script>
export default{
    name: 'ConvertirTiempo',
    data(){
        return{
            vEntrada: '',
            resultado: ''
        }
    },
    methods:{
        Calculartiempo(){
            this.resultado = this.vEntrada * 60;
            console.log(this.vEntrada);
            console.log(this.resultado)
        }
    }
}
</script>
