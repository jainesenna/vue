<template>
    <div>
        <input v-model="valor" />
        <p v-if="valorQuadrado % 2 === 0">{{valorQuadrado}}</p>
    </div>
</template>
<script>
export default {
    data(){
        return{
            valor: 0
        }
    },
    computed: {
        valorQuadrado(){
            return Math.pow(this.valor, 2)
        }
    },
    methods:{

    }
}
</script>