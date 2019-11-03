<template>
  <div class="resgistration-cube registration-grid">
    <div class="first-name">
      <label for="fname">First Name</label>
      <input class="input-style" type="text" id="fname" name="firstname" />
    </div>
    <div class="last-name">
      <label for="lname">Last Name</label>
      <input class="input-style" type="text" id="lname" name="lastname" />
    </div>
    <div class="company">
      <label for="company">Company</label>
      <input class="input-style" type="text" id="company" name="company" />
    </div>
    <div class="email">
      <label for="email">Email</label>
      <input
        v-on:change="UpdateErrorMessage"
        v-model="emailAddress"
        class="input-style"
        type="text"
        id="email"
        name="email"
      />
      <div v-if="errorMsg" class="error-message">Invalid Email address</div>
    </div>
    <div class="register-input">
      <button v-on:click="RegisterUser" class="register-btn">Register</button>
    </div>
  </div>
</template>
<script>
export default {
  name: "Register",
  data: () => ({
    emailAddress: "",
    errorMsg: false
  }),
  methods: {
    RegisterUser() {
      // chek other data
      if (!this.validEmail(this.emailAddress)) this.errorMsg = true;
    },

    validEmail(email) {
      var re = /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
      return re.test(email);
    },
    UpdateErrorMessage() {
      this.errorMsg = false;
    }
  }
};
</script>
<style scoped>
.resgistration-cube {
  background: white;
  height: 100%;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
}
.registration-grid {
  display: grid;
  grid-template-columns: 50% 50%;
  align-items: center;
}
.first-name {
  grid-column-start: 1;
  grid-column-end: 1;
  grid-row-end: 1;
  grid-row-start: 1;
  margin-left: 20%;
  padding-right: 20px;
}
.last-name {
  grid-column-start: 2;
  grid-column-end: 2;
  grid-row-end: 1;
  grid-row-start: 1;
  margin-right: 20%;
  padding-left: 20px;
}
.company {
  grid-column-start: 1;
  grid-column-end: 3;
  grid-row-end: 2;
  grid-row-start: 2;
  display: inline-grid;
  margin-right: 10%;
  margin-left: 10%;
}
.email {
  grid-column-start: 1;
  grid-column-end: 3;
  grid-row-end: 3;
  grid-row-start: 3;
  display: inline-grid;
  margin-right: 10%;
  margin-left: 10%;
}
.register-btn {
  background-color: #00b5ef;
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}
.register-input {
  grid-column-start: 1;
  grid-column-end: 1;
  grid-row-end: 4;
  grid-row-start: 4;
}
.input-style {
  color: #333;
  float: left;
  font-family: Helvetica, Arial, sans-serif;
  font-size: 18px;
  line-height: 40px;
  margin: 0 20px 10px;
  width: 100%;
}
.error-message {
  color: #ff0040;
  display: inline-block;
  font-size: 20px;
  line-height: 15px;
  margin: 5px 0 0;
  margin-right: 10px;
}
</style>