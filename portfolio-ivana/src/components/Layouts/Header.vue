<template>
  <b-navbar
    toggleable="md"
    type="dark"
    variant="faded"
    style="padding: 15px; background-color: #3f3f3f !important"
  >
    <b-navbar-brand href="#" class="custom-nav-brand">Ивана Коцева</b-navbar-brand>

    <!-- <b-navbar-toggle target="nav-collapse"></b-navbar-toggle> -->

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav style="justify-content: flex-end">
      <b-navbar-nav>
        <b-nav-item
          v-for="item in menuItems"
          :key="item.href"
          :href="item.href"
          class="custom-nav-item"
        >
          {{ item.text }}
        </b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {
  data() {
    return {
      menuItems: [
        { href: '#whatyouget', text: 'Што добивате вие' },
        { href: '#about', text: 'За мене' },
        { href: '#contact', text: 'Контактирајте ме' }
      ]
    }
  }
}
</script>

<style scoped>
.custom-nav-item >>> .nav-link {
  color: white !important; /* Ensures that the text color is applied */
}
.navbar-brand {
  color: white !important;
}

.custom-nav-item >>> .nav-link:hover {
  color: #007bff !important; /* Change text color on hover */
}
.navbar-toggler {
  border: none;
}

.navbar-toggler:focus {
  text-decoration: none;
  outline: 0;
  color: white !important;
  box-shadow: 0 0 0 var(--bs-navbar-toggler-focus-width);
}
.custom-nav-item >>> .nav-link.active {
  color: #adb5bd !important; /* Change text color for the active nav item */
}
</style>
