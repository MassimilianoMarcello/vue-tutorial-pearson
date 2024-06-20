<template>
    <div>
<h1 v-if="showFlashMessage">{{ message }}</h1>
    </div>
</template>

<script>
    export default {
        name:'flash message',
        props:['message','delay'],
        data(){
            return{
                showFlashMessage: true,
            
            }
           
        },
        
        
        created(){
            setInterval(() => {
      this.showFlashMessage=!this.showFlashMessage
        }, this.delay);
        }
    }
</script>