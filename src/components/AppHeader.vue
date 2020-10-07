<template>
  <div>
  <b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand class="brand"><img src="@/assets/logo.jpg" /></b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">     
            <b-nav-item @click="toHome">Home</b-nav-item>
            <b-nav-item @click="toAbout">About</b-nav-item>
            <b-nav-item @click="toBackground">Background</b-nav-item>
            <b-nav-item @click="toPortfolio">Portfolio</b-nav-item>
            <b-nav-item @click="toContact">Contact</b-nav-item>
        </b-navbar-nav>
    </b-collapse>
   
  </b-navbar>
</div>
</template>

<script>
export default {
  name: 'appHeader',
  components: {
  },
  methods: {
    toHome () {
      this.$router.push({ name: 'Home' })
    },
    toAbout () {
      this.$router.push({ name: 'About' })
    },
    toBackground () {
      this.$router.push({ name: 'Background' })
    },
    toPortfolio () {
      this.$router.push({ name: 'Portfolio' })
    },
    toContact () {
      this.$router.push({ name: 'Contact' })
    },
  }
}
</script>

<style scoped lang="less">
.brand img {
    width: 60px;
    height: 50px;
    border-radius: 50%;
    margin-left: 3vw;   
}
.ml-auto {
    margin-right: 3vw;
    .nav-item {
        padding: 0 20px 0 20px;
        ;
    }
}
.navbar {
    z-index: 2;
}

</style>