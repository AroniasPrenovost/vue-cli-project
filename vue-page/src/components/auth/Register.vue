<template>
   <div>
       <h3 class='text-center'>Register</h3>
       
       <input type='text' class='form-control m-b-15' placeholder='Email Address' v-model='user.email'>
       <input type='text' class='form-control m-b-15' placeholder='Username' v-model='user.username'>
       <input type='text' class='form-control m-b-15' placeholder='Password' v-model='user.password'>
       
       <hr>
       
       <button class='btn btn-lg btn-primary btn-black m-b-15 @click=register'>Register</button>
       <!-- @click is short for v-on:click -->
       <p class='text-center'>
           Already have an account? <router-link to ='/auth/login'>Login!</router-link>
       </p>
   </div>
</template>

<script>
    export default {
      name: 'register',
      data: function () {
        return {
          user: {
            email: '',
            username: '',
            password: ''
          }
        }
      },
      methods: {
        register: function () {
          console.log(this.user)
        }
      }
    }
</script>

<style>
    
</style>
