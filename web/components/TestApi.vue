<template>
    <div style="text-align:center; margin-top:20rem;">
        <h1>This is Res :</h1>
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
    async created() {
        await this.$axios.get("http://api:8000/").then((res) => {   
            console.log(res);
            this.res = res
      }).catch((err) => {
        this.res = err
      });
    },
}
</script>