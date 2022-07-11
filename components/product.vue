<template >
    <div>
        <div class="row">
            <div class="col-4" v-if="en">
                <div class="card" style="width: 18rem;">
                    <img src="~/assets/img/brainstorming.png" class="card-img-top" alt="product image">
                    <div class="card-body">
                        <h5 class="card-title">Card title</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="btn btn-primary">Go somewhere</a>
                    </div>
                </div>
            </div>
            <div class="col-4" v-if="bd">
                <div class="card" style="width: 18rem;">
                    <img src="~/assets/img/brainstorming.png" class="card-img-top" alt="product image">
                    <div class="card-body">
                        <h5 class="card-title">bangla</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="btn btn-primary">Go somewhere</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:'Product',
    data(){
        return{
            bd:false,
            en:true
        }
    },
    created(){
        if(this.$i18n.locale == 'bd'){
            this.bd = true;
            this.en = false;
        }
        else{
            this.en = true;
            this.bd = false;
        }
        
    }
}
</script>
<style lang="">
    
</style>