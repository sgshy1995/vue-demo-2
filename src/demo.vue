<template>
  <div>
    <div>{{displayName}}</div>
    <button @click="transform">transform</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      user: {
        name: "eden",
        email: "singlesaul@163.com",
        phone: "15000856717"
      }
    };
  },
  computed: {
    displayName: {
      get() {
        return this.user;
      },
      set(value) {
        this.user.name = value;
      }
    }
  },
  methods: {
    transform() {
        this.displayName = 'sgs'
    }
  }
};
</script>

<style scoped>
</style>