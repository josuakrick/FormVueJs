<template>
<section class="mx-8 my-6 md: flex-1">
    <button class="my-8 p-6 bg-violet-700 text-white rounded-lg hover:bg-violet-500">
       <b>Try it free 7 days</b> then $20/mo. thereafter
    </button>
<form action="submit" class="flex flex-col gap-y-4 bg-slate-50 px-6 py-8 rounded-lg">
  <input type="text" alt="name" :placeholder='first_name' required>
  <input type="text" alt="lastname" :placeholder="last_name" required>
  <input type="email" alt="email" :placeholder="email"  required>
  <input type="password" alt="password" :placeholder="password" pattern="^(?=.*[a-z])(?=.*[A-Z])(?=.*[0-9])(?!.*[ !@#$%^&*_=+-]).{6,12}$" required>
  <button class="bg-green-500 py-6 rounded-lg text-white font-bold hover:bg-green-700">Claim your free trial!</button>
  <p class="pt-4 px-6 opacity-70">By clicking the button, you are agreeing to our <a href="#" class="text-red-600 opacity-1 font-bold hover:text-red-400">Terms and Services</a></p>
</form>

</section>
</template>
<!-- <img src="../../public/icon-error.svg" alt=""></img> -->

<script>

export default {
  name: 'One_Form',
  data() {
    return {
        first_name: 'First Name',
        last_name: 'Last Name',
        email: 'Email Address',
        password: 'Password',
        vazio: ''
    }
  },
}
</script>

<style lang="scss">
section {
  button {
    width: 100%;
  }
  form {
    input {
      padding: 1rem;
      border: rgb(206, 205, 205) 1px solid;
      border-radius: 0.5rem;
    }
    input::placeholder {
      color: black;
      font-weight: 600;
      opacity: 0.7;
    }
    input:invalid {
      border-color: rgb(250, 100, 100);
    }
  }
}
</style>

