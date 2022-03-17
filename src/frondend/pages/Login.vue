<template>
  <div>
    <div class="page-section">
      <div class="container">
        <h1 class="text-center wow fadeInUp">Login</h1>

        <div class="row mb-3 text-left justify-content-md-center">
          <div class="col-6 py-3 contact-form mt-5 card rounded wow fadeInUp" style="border: 1px solid #d7c5c5">
            <div class="py-2">
              <label for="subject">Email</label>
              <input
                type="text"
                id="subject"
                class="form-control"
                placeholder="Enter Email.."
              />
            </div>

            <div class="py-2">
              <label for="subject">Password</label>
              <input
                type="text"
                id="subject"
                class="form-control"
                placeholder="Enter Password.."
              />
            </div>

            <div class="row justify-content-center mt-3">
                <button class="btn btn-primary" @click="login">Login</button>
            </div>
            <div class="row justify-content-center mt-3">
                <a href="/register">Don't have account?</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
export default {
    methods: {
        login() {
            // eslint-disable-next-line no-console
            console.log('login')
            this.$router.push({path: '/home'})
        }
    }
}
</script>