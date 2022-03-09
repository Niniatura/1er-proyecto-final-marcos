<template>
  <v-app>
    <v-card class="register-form">
      <v-window v-model="step">
      <v-window-item :value="1">
        <v-card-title>
          <h1>Register</h1>
        </v-card-title>
        <v-card-text>
          <v-form>
            <v-text-field label="Username" prepend-icon="mdi-account-circle"/>
            <v-text-field
              v-model="email"
              :error-messages="emailErrors"
              label="Email"
              required
              prepend-icon="mdi-mail"
          />
            <v-text-field 
              :type="showPassword ? 'text' : 'password'" 
              prepend-icon="mdi-lock" append-icon="mdi-eye-off"
              label="Password"
              @click:append="showPassword = !showPassword" 
            />
          </v-form>
        </v-card-text>
        <v-card-actions>
          <v-btn @click="step++">Login</v-btn>
          <v-spacer></v-spacer>
          <v-btn>Register</v-btn>
        </v-card-actions>
      </v-window-item>
      <v-window-item :value="2">
        <v-card-title>
          <h1>Login</h1>
        </v-card-title>
        <v-card-text>
          <v-form>
            <v-text-field label="Username" prepend-icon="mdi-account-circle"/>
            <v-text-field 
              :type="showPassword ? 'text' : 'password'" 
              prepend-icon="mdi-lock" append-icon="mdi-eye-off"
              label="Password"
              @click:append="showPassword = !showPassword" 
            />
          </v-form>
        </v-card-text>
         <v-card-actions>
          <v-btn @click="step--">Register</v-btn>
          <v-spacer></v-spacer>
          <v-btn>Login</v-btn>
        </v-card-actions>
      </v-window-item>
      </v-window>
      </v-card>
  </v-app>
</template>

<script>

export default {
    name:'FormRegistro',
    data: () => ({
    step: 1,
    showPassword: false
  }),
  props: {
    source: String
  }
}
</script>

<style scoped>
.register-form{
  max-width: 75%;
  margin-left: 15% !important;
}
</style>
