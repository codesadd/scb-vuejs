<template>
  <div id="login">
    <section class="hero is-primary is-fullheight">
      <div class="hero-body">
        <div class="container">
          <div class="columns">
            <div class="column is-two-thirds has-text-centered">
              <h1 class="title">
                SCB ไทยพาณิชย์
              </h1>
              <h2 class="subtitle">
                Universal Convertor
              </h2>
            </div>
            <div class="column">
              <div class="box is-primary">
                <div class="field">
                  <p class="control has-icons-left has-icons-right">
                    <input class="input" type="text" placeholder="Corp ID" v-model="corpId">
                    <span class="icon is-small is-left">
                      <i class="fas fa-envelope"></i>
                    </span>
                    <span class="icon is-small is-right">
                      <i class="fas fa-check"></i>
                    </span>
                  </p>
                </div>
                <div class="field">
                  <p class="control has-icons-left">
                    <input class="input" type="text" placeholder="User" v-model="username">
                    <span class="icon is-small is-left">
                      <i class="fas fa-lock"></i>
                    </span>
                  </p>
                </div>
                <div class="field">
                  <p class="control has-icons-left">
                    <input class="input" type="password" placeholder="Password" v-model="password">
                    <span class="icon is-small is-left">
                      <i class="fas fa-lock"></i>
                    </span>
                  </p>
                </div>
                <div class="field">
                  <p class="control">
                    <button class="button is-success" @click="login">
                      Login
                    </button>
                  </p>
                </div>
              </div>

            </div>
          </div>
        </div>


      </div>
    </section>
  </div>
</template>

<script>
  export default {
    name: 'Login',
    data() {
      return {
        corpId: 'LAPSCBComp09',
        username: 'maker05',
        password: '123'
      }
    },
    methods: {
      login() {
        if (this.corpId == "LAPSCBComp09" && this.username == "maker05") {
          alert("Login Success")
        }
      }
    }
  }
</script>

<style scoped>
</style>