<template>
    <div>
        <br>
        <br>
        <h2>Megabytes a Gigabytes</h2>
        <input v-model="vEntrada" type="numbre" placeholder="Ingrese el numero de megas a convertir"/>
        <br>
        <b-button variant="success" v-on:click="Calcularalmacenamiento" title="Convertir">Convertir</b-button>
        <br>
        <h4>{{vEntrada}} megabytes equivalen a: {{resultado}} gigabytes</h4>

    </div>
</template>
<script>
export default{
    name: 'ConvertirAlmacenamiento',
    data(){
        return{
            vEntrada: '',
            resultado: ''
        }
    },
    methods:{
        Calcularalmacenamiento(){
            this.resultado = this.vEntrada * 0.001;
            console.log(this.vEntrada);
            console.log(this.resultado)
        }
    }
}
</script>
