<template>
  <div class="profile-container">
    <img :src="user.picture" alt="User Picture" class="profile-picture">
    <h2 class="profile-name">{{ user.name }}</h2>
    <p class="profile-email">{{ user.email }}</p>
    <p class="profile-nickname">{{ user.nickname }}</p>
    <p class="profile-locale">{{ user.locale }}</p>
    <p class="profile-updated">{{ user.updated_at }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      user: {},
    };
  },
  mounted() {
    this.user = this.$auth.user;
  },


};
</script>

<style scoped>
.profile-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background-color: #f5f5f5;
  font-family: Arial, sans-serif;
}

.profile-picture {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  object-fit: cover;
}

.profile-name {
  color: #333;
  font-size: 2em;
  margin-top: 20px;
}

.profile-email, .profile-nickname, .profile-locale, .profile-updated {
  color: #666;
  font-size: 1em;
  margin-top: 10px;
}
</style>