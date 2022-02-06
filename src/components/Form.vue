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
      <p>SELECTION</p>
      <select v-model="role">
        <option value="developer">Web Developer</option>
        <option value="designer">Web Designer</option>
      </select>
    </form>
    <div>
      <p>Email: {{ email }}</p>
      <p>Password: {{ password }}</p>
      <p>Role: {{ role }}</p>
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
      role: "",
    };
  },
};
</script>

<style scoped></style>
