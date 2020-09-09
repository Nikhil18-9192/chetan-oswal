<template>
<div>
     <div class="top-header">
         <div class="container">
             <div class="links">
                 <div class="email">
                     <div class="logo">
                        <img src="/envelop.svg" alt="img">
                 </div>
                 <div class="text">
                     <a href="mailto: ca.chetanoswal@gmail.com">{{ contactInfo.mail }}</a>
                 </div>
                 </div>
                  <div class="email">
                     <div class="logo">
                         <img src="/phone.svg" alt="img">
                 </div>
                 <div class="text">
                    <a href="tel:+919890828242">{{ contactInfo.phone }}</a>
                 </div>
                 </div>
                 
             </div>
         </div>
     </div>
</div>
</template>
<script lang="ts">
import Vue from 'vue'
import contactInfo from '../utils'
export default Vue.extend ({
    
    data(){
        return{
            contactInfo:{
                 mail:'ca.chetanoswal@gmail.com',
                 phone: '+91 9890 828242'
                }
              }
            }
});
</script>
<style lang="scss" scoped>
.top-header{
    background: #f2f2f2;
    padding: 10px;
    
    .link{
        display: flex;

        .email{
            display: flex;
        }
    }
}
</style>