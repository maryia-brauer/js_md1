<template>
  <div>
    <h1>ABOUT ME</h1>
    <h3>Name: {{ user.name }}</h3>
    <h3>Surname: {{ user.surname }}</h3>
    <h3>Code: {{ user.code }}</h3>
  </div>
</template>

<script>
export default {
  data() {
    return {
      user: {
        name: "Maryia",
        surname: "Brauer",
        code: "IT21057"
      }
    };
  }
};
</script>
