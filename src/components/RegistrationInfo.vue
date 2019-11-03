<template>
  <div>
    <div class="empty-grid-item"></div>
    <div class="grid-item">
      <div class="info">
        <img class="img-logo" alt="Atom logo" src="./../assets/aton.png" />
        <p class="grid-text">Centralizez comunication channers and reduces overhead.</p>
      </div>
    </div>
    <div class="grid-item">
      <div>
        <div class="info">
          <img class="img-logo" alt="Atom logo" src="./../assets/chat.png" />
          <p
            class="grid-text"
          >Brings together instant messaging, voice and video communication in the browser.</p>
        </div>
      </div>
    </div>
    <div class="grid-item">
      <div class="info">
        <img class="img-logo" alt="Atom logo" src="./../assets/settings.png" />
        <p
          class="grid-text"
        >Captures information across the organization, retains the knowledge, abalyzes and improves it.</p>
      </div>
    </div>

    <div class="help-row">
      <div class="info">
        <img class="help-img-logo" alt="Atom logo" src="./../assets/help-logo.png" />
        <p class="grid-text">
          <b>+1 845 894 123</b>
          <br />
          <a href="mailto:help@hubgets.com">help@hubgets.com</a>
        </p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "RegistrationInfo",
  props: {}
};
</script>
<style scoped>
.grid-container {
  display: grid;
  grid-template-columns: auto;
  padding: 10px;
}
.grid-item {
  padding: 15px;
  text-align: left;
}
.empty-grid-item {
  height: 5em;
}

.info {
  display: flex;
}
.img-logo {
  height: 60px;
  vertical-align: -0.8em;
}
.grid-text {
  margin-left: 2%;
}
.help-row {
  padding: 30px;
  text-align: left;
}
.help-img-logo {
  height: 70px;
  vertical-align: -0.8em;
}
</style>