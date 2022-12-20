<template>
<div class="root">
  <label>
    Введите email:
    <input
      type="email"
      :value="email"
      @input="emailInput($event.target.value)"
    />
    {{ email }}
  </label>
  <label>
    Введите пароль:
    <input type="password"
    :value="password"
    @input="inputPassword($event.target.value)"
    />
  </label>
  email: {{ email }}
  password: {{ password }}
</div>
</template>
<script>
export default {
  name: "MyComponent",
  data(){
    return {
      email: 'mycomponent@mail.com',
      password: '123456789'
    }
  },
  methods: {
    emailInput(value) {
      this.email = value
      // console.log(event.target.value);
    },
    inputPassword(value) {
      this.password = value

    }
  }
}
</script>