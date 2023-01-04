<script setup>
// import { RouterLink, RouterView } from 'vue-router'
// import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div class="container">
    <div class="section-ilustration">
      <div class="navbar-left">
        <img src="./assets/logo.svg" alt="">
        <img src="./assets/Digicoins.svg" alt="">
      </div>
      <div class="container-illustration">
        <img
          class="illustration-img"
          src="./assets/illustration-signup.png"
          alt=""
        >
      </div>
    </div>
    <div class="section-form">
      <div class="navbar-right">
        <p>EN/USD</p>
        <span>|</span>
        <img src="./assets/dark-light.svg" alt="">
      </div>
      <div class="user-have-account">
        <p>Already have an account? <span class="login"><a href="/login">Login</a></span></p>
      </div>
      <div class="form-input">
        <h2 class="sign-up-title">Sign Up</h2>
        <p>Use Your OpenID to Sign up</p>
        <div class="user-select">
          <p>Email</p>
          <span>|</span>
          <p>Phone Number</p>
        </div>
        <form class="form" action="" @submit.prevent="">
          <div class="email-form">
            <label for="email">Email</label>
            <input class="input" type="email">
          </div>
          <div class="email-form passsword-form">
            <label for="password">Password</label>
            <input class="input" type="password">
          </div>
          <div class="email-form passsword-form">
            <label for="password">Confirmation Password</label>
            <input class="input" type="password">
          </div>
          <div class="referal-id">
            <p>Referal ID (Optional)</p>
            <img src="./assets/drop-down.svg" alt="">
          </div>
          <div class="user-agreements">
            <input type="checkbox">
            <div>
              <p>By signing up I agree that I’m 18 years of age or older, to the User Agreements, Privacy Policy, Cookie Policy, E-Sign Consent.</p>
            </div>
          </div>
          <button type="submit">Sign Up</button>
        </form>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  width: 100vw;
  height: 100vh;
}
.section-ilustration {
  background-color: #0E1114;
  width: 60%;
}

.navbar-left {
  display: flex;
  align-items: center;
  padding: 10px;
  gap: 10px;
}
.container-illustration {
  display: flex;
  justify-content: center;
  align-items: center;
}

.illustration-img {
  width: 70%;
  object-fit: cover;
}

/* Right */
.section-form {
  background-color: #1E1E1E;
  width: 100%;
  color: #FFF;
  padding: 10px 40px 0 20px;
}

.navbar-right {
  display: flex;
  justify-content: right;
  align-items: center;
  gap: 20px;
  width: 100%;
}

.user-have-account {
  margin-top: 10px;
  text-align: right;
}

.login a {
  color: #02C3BD;
  text-decoration: none;
}
.login a:hover{
  cursor: pointer;
}

.form-input {
  margin: 20px 0 0 40px;
}

.form-input p {
  margin-top: 8px;
}

.sign-up-title {
  font-size: 30px;
  font-weight: 500;
}

.user-select {
  display: flex;
  align-items: center;
  gap: 20px;
  margin: 20px 0;
}

.user-select p:hover {
  color: #02C3BD;
  cursor: pointer;
}
.user-select span {
  margin-top: 5px;
}

.email-form {
  display: flex;
  flex-direction: column;
  gap: 5px;
}

.form {
  width: 350px;
}

.input {
  width: 100%;
  padding: 12px;
  border: 1px solid #FFF;
  background: transparent;
  border-radius: 5px;
  color: #FFF;
}

.input:focus {
  outline: none;
}

.passsword-form {
  margin: 10px 0 0 0;
}
.referal-id {
  display: flex;
  align-items: center;
  margin: 10px 0 0 0;
  gap: 10px;
}
.referal-id img {
  margin-top: 10px;
}

.user-agreements {
  display: flex;
  gap: 15px;
}
button {
  background: linear-gradient(135deg, #02C3BD 0%, #4062BB 100%);
  width: 100%;
  padding: 10px;
  border: none;
  border-radius: 4px;
  color: #FFF;
  font-weight: 600;
  margin: 10px 0;
}
button:hover {
  cursor: pointer;
}
</style>
