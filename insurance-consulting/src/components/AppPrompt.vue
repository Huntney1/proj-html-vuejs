<script>
export default {
   name:'AppPrompt',
   data() {
    return {
        number: 0
    }
   }, 
   methods: {
        increment() {
            this.number++;
        },
        decrement() {
            this.number--;
        }
    },
};
</script>

<template lang="">
    <div class="continer">
        
        <div class="row">
            <!-- 1° sezione text -->
            <div class="col-12 col-md-6 input-group text-left">
                <h6>FUSION & ACQUISTIONS</h6>
                <h1>Insurance Consulting</h1>
            </div>
            
            <!-- 2° sezione input -->  
            <div class="col-12 col-md-6 input-group">
                <input type="text" class="form-control" placeholder="Name">
                <input type="text" class="form-control" placeholder="Email">
            </div>
        
            <div class="col-12 col-md-6 input-group">
               
                <div>
                    <div @click="decrement"></div>
                    <input type="number" v-model="number" placeholder="phone" class="form-control">
                    <div @click="increment"></div>
                </div>


                <!-- <select class="form-control">
                    <option value="" disabled selected>Phone</option>
                    <option value="opzione1">Opzione 1</option>
                    <option value="opzione2">Opzione 2</option>
                    <option value="opzione3">Opzione 3</option>
                </select> -->

               
            </div>
            <div class="col-12 col-md-6 input-group">
                
            


            </div>
            
            
        </div>
        
    </div>
</template>

<style lang="scss" scoped>

</style>
