<template>
  <div
    class="flex-none md:flex justify-center text-center items-center h-screen"
  >
    <div class="w-full md:w-3/4 lg:w-1/2 xl:w-2/6">
      <rs-card class="h-screen md:h-auto px-10 md:px-16 py-12 md:py-20 mb-0">
        <h3 class="mb-4">Forgot Password</h3>
        <p class="text-slate-500 mb-6">
          Please input the correct email to reset the password.
        </p>
        <div class="grid grid-cols-1">
          <FormKit label="Email" type="email" outer-class="text-left" />
          <router-link :to="{ name: 'auth-resetpasswordv2' }">
            <FormKit type="button" input-class="w-full">Validate Email</FormKit>
          </router-link>
        </div>
        <p class="mt-3 text-center text-slate-500">
          Already have an account?
          <router-link
            :to="{ name: 'auth-loginv2' }"
            class="text-primary-400 hover:underline"
            >Login</router-link
          >
        </p>
      </rs-card>
    </div>
  </div>
</template>

<script>


export default {
  
  setup() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
</style>