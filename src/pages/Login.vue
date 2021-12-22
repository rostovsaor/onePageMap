<template>
  <div class="q-ma-md">
    <nav class="flexbox row items-center q-mb-md">
      <q-icon class="my-grey" name="arrow_back" size="2rem"/>
      <p class="my-grey ">Insira suas credenciais</p>
    </nav>
    
    <div class="container q-mb-lg bg-grey-1">
      <q-input class="input q-pl-md" borderless placeholder="Username ou email" v-model="user" />
      <q-separator />
      <q-input class="input q-pl-md" borderless type="password" placeholder="Palavra Passe" v-model="pass"/>
    </div>
    
    <q-btn class="login q-mb-lg" flat >Login</q-btn>

    <q-btn class="reset q-mb-lg" flat >Esqueci a Palavra Passe</q-btn>

    <!-- <div class="a">
      <a href="" style="">Esqueci a Palavra Passe</a>
    </div> -->
  </div>
</template>

<script>
import { ref } from 'vue'
export default {
  name: 'Login',
  setup () {
    return {
      user: ref(''),
      pass: ref('')
    }
  }
}
</script>


<style>
  .container {
    border-style: solid;
    border-color: rgb(224, 224, 224);
    border-width: 0.18rem;
    border-radius: 1.4em;
  }

  span { 
    font-weight: 600;
    /* margin: 0 auto; */
  }

  .my-grey {
    color: rgb(175, 175, 175) ;
  }

  p {
    margin: 0 auto;
    font-size: 1.6rem;
    font-weight: 800;
  }

  q-input {
    font-size: 3rem;
    color: aqua;
    background_color: blue;
  }

  .login { 
    width: 100%;
    padding: 0.5em 0;
    font-size: 1.5rem;
    font-weight: 600;
    color: rgb(175, 175, 175);
    background-color: rgb(227, 227, 227);
    border-radius: 0.8em;
  }
  
  .reset { 
    width: 100%;
    padding: 0.5em 0;
    font-size: 1.5rem;
    font-weight: 600;
    color: rgb(28, 176, 246);
    border-radius: 0.8em;
  }

  .a, a {
    text-decoration: none;
    margin: 0 auto;
  }
</style>