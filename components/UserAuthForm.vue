<template>
	<div>
		<div class="container">
			<div class="is-centered columns">
				<div class="column is-6	">
					
					<form>


          

            <div class="field">
              <label class="label">Email</label>
              <div class="control has-icons-left has-icons-right">
                <input class="input " type="email" placeholder="Email " v-model="email" name="email">
                <span class="icon is-small is-left">
                  <i class="fas fa-envelope"></i>
                </span>
                <span class="icon is-small is-right">
                  <i class="fas fa-exclamation-triangle"></i>
                </span>
              </div>
              <!-- <p class="help is-danger">This email is invalid</p> -->
            </div>


            <div class="field">
              <label class="label">Password</label>
              <div class="control has-icons-left has-icons-right">
                <input class="input " type="text" v-model="password" name="password" placeholder="Password" value="">
                <span class="icon is-small is-left">
                  <i class="fas fa-user"></i>
                </span>
                <span class="icon is-small is-right">
                  <i class="fas fa-check"></i>
                </span>
              </div>
            </div>


            <div class="field">
              <button class="button is-primary" @submit="Login">Login</button>
            </div>


					</form>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
  export default {
    data () {
      return {
        email: '',
        password: '', 
      }
    },

    methods: {
      login() {
        alert('loggin in')
      }
    }
  };
</script>