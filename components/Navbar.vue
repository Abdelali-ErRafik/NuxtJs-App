<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark padding">
    <div class="container">
      <NuxtLink class="navbar-brand" to="/">Firengi</NuxtLink>
      <button class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse ml-auto" id="navbarSupportedContent">
          <ul class="navbar-nav ml-auto">
              <li class="nav-item active">
                  <NuxtLink to="/products" class="nav-link">Products <span class="sr-only">(current)</span></NuxtLink>
              </li>
              <li class="nav-item active">
                  <NuxtLink to="/my-items" class="nav-link">My Items <span class="sr-only">(current)</span></NuxtLink>
              </li>
          </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavbarView'
}
</script>

<style scoped>
    .padding {
        padding: 1rem;
        background-color: black
    }
    .nav-left {
        margin-left: auto;
    }
</style>
