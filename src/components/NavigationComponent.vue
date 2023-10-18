<template>
  <div>
    <ul class="tabs">
      <li :class="{ active: activeTab === 'home' }" @click="changeTab('home')">HOME</li>
      <li :class="{ active: activeTab === 'about' }" @click="changeTab('about')">ABOUT ME</li>
    </ul>
  </div>
</template>



<script>
export default {
  props: {
    activeTab: String
  },
  methods: {
    changeTab(tab) {
      this.$emit('tab-change', tab);
    }
  }
};
</script>

<style scoped>
ul.tabs {
  list-style-type: none;
  padding: 0;
}

ul.tabs li {
  margin-bottom: 10px;
  cursor: pointer;
}

ul.tabs li.active {
  border-bottom: 2px solid white;
  background-color: purple;
}
</style>
