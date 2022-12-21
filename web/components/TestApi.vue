<template>
    <div style="text-align:center;">
        {{ api }}
    </div>
</template>

<script>
export default {
    data(){
        return{
            res:null
        }
    },
    computed: {
        api(){
            return this.res
        }
    },
    created() {
        this.$axios.get('http://api:8000/api/v1').then(res)=>({
            this.res = res
        }).catch(err)=>({
            this.res = res
        })
    },
}
</script>