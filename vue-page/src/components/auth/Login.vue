<template>
   <div>
       <h3 class='text-center'>Login</h3>
       
       <input type='text' class='form-control m-b-15' placeholder='Username'>
       <input type='text' class='form-control' placeholder='Password'>
       
       <hr>
       
       <button class='btn btn-lg btn-primary btn-black m-b-15'>Sign in</button>
       <p class='text-center'>
           Don't have an account? <router-link to ='/auth/register'>Sign Up!</router-link>
       </p>
   </div>
</template>

<script>
    export default {
      name: 'login'
    }
</script>


<style>
    
</style>
