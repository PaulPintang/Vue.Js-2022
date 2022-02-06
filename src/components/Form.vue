<template>
  <div style="padding-top: 20px">
    <form action="">
      <input type="email" placeholder="Email" v-model="email" required />
      <input
        type="password"
        placeholder="Password"
        v-model="password"
        required
      />
    </form>
    <div>
      <p>Email: {{ email }}</p>
      <p>Password: {{ password }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Form",
  data() {
    return {
      email: "",
      password: "",
    };
  },
};
</script>

<style scoped></style>
