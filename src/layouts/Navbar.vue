<template>
  <nav class="navbar navbar-expand-md navbar-light bg-white shadow-sm px-md-0 px-sm-2 py-md-2 py-sm-2">
    <div class="container-fluid md:row d-md-flex justify-content-between px-md-5">
      <div class="d-flex justify-content-start align-items-center gap-2">
        <g-image alt="multividas, multividas api documentation, multividas threads, multividas status, multividas help center, multividas developer, multividas about us, multividas ads, multividas engineering blog, multividas developers documentation, multividas embed threadsmultividas, multividas api documentation, multividas threads, multividas status, multividas help center, multividas developer, multividas about us, multividas ads, multividas engineering blog, multividas developers documentation, multividas embed threadsmultividas, multividas api documentation, multividas threads, multividas status, multividas help center, multividas developer, multividas about us, multividas ads, multividas engineering blog, multividas developers documentation, multividas embed threadsmultividas, multividas api documentation, multividas threads, multividas status, multividas help center, multividas developer, multividas about us, multividas ads, multividas engineering blog, multividas developers documentation, multividas" src="~/assets/png/nav-logo.png" width="35" />
        <strong>
          <g-link to="/" class="navbar-brand text-primary fw-bold fs-4">About</g-link>
        </strong>
      </div>

      <div class="navbar-block show-on-medium">
        <ul class="navbar-nav d-flex justify-container-end align-items-center gap-4">
          <li class="nav-item">
            <g-link class="nav-link" to="/resources/about-us">About us</g-link>
          </li>
          <li class="nav-item">
            <g-link class="nav-link" to="/resources/brand-toolkit">Brand toolkit</g-link>
          </li>
          <li class="nav-item">
            <a class="btn btn-sm btn-light border text-xxs fw-medium px-3 py-2 rounded-4" href="https://multividas.com/"
              target="_blank">
              Go to Multividas.com
            </a>
          </li>
        </ul>
      </div>
      <!--  -->
      <div class="navbar-block show-on-small">
        <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas"
          data-bs-target="#offcanvasMultividasNavbar" aria-controls="offcanvasMultividasNavbar">
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="offcanvas offcanvas-start" tabindex="-1" id="offcanvasMultividasNavbar"
          aria-labelledby="offcanvasMultividasNavbarLabel">
          <div class="offcanvas-header">
            <h5 @click="redirectRoute('/')" role="button" class="offcanvas-title text-primary fw-bold"
              id="offcanvasMultividasNavbarLabel">
              About
            </h5>
            <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
          </div>
          <div class="offcanvas-body p-0">
            <ul class="navbar-nav d-flex justify-container-end align-items-center gap-md-4">
              <li class="nav-item border-top border-bottom w-100 w-full text-center">
                <span class="nav-link" @click="redirectRoute('/resources/about-us')"
                  :class="{ 'active--exact active': $route.path === '/resources/about-us' }" role="button">About us</span>
              </li>
              <li class="nav-item border-bottom w-100 w-full text-center">
                <span class="nav-link" @click="redirectRoute('/resources/brand-toolkit')" :class="{
                  'active--exact active': $route.path === '/resources/brand-toolkit',
                }" role="button">Brand toolkit</span>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  methods: {
    redirectRoute(name) {
      return (window.location.href = name);
    },
  },
};
</script>

<style scoped>
/* Default styles for all screen sizes */
.navbar-block {
  display: none;
}

/* Display elements on small screens */
@media (max-width: 767px) {
  .show-on-small {
    display: block;
  }
}

/* Display elements on medium and larger screens */
@media (min-width: 768px) {
  .show-on-medium {
    display: block;
  }
}
</style>
