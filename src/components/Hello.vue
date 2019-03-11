<template>
   <div id="app">
            <input type="text" v-model="message2"/>
            <p
                v-html="
                    message1.slice(0, 7) +
                    message2 +
                    message1.slice(12)
            "></p>
   </div>
</template>
<script>

export default {
   name: 'Hello',
   data(){
       return{

               message1: "Hello, World!",
               message2: "Vue"

       }
   }
}
</script>


<style scoped>

/* resets */
* { color: inherit; }
input { font: inherit; border: unset; background: unset; }
input:focus { outline: unset; }

:root {
    font: 1rem/1.175 "BlinkMacSystemFont", -apple-system, "Roboto", sans-seri;
}

#app {
     display: flex;
    flex-direction: column; 
     justify-content: center; 
    align-items: center; 
     width: 46vw; height: 100vh;
    /* width: 60vw; */
    margin-left: -40vw;
    margin: 0vw;
    font-weight: 900; font-size: 4rem;
    color: hsl(0, 0%, 100%);
    background: hsl(240, 100%, 67%);
}

input { text-align: center; }

img {
    width: 8rem; height: 8rem;
    vertical-align: calc(-0.12109375em);
}

</style>