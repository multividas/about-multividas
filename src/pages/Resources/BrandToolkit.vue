<template>
  <MainLayout>
    <header class="mv-header mv-header-bg px-3 px-sm-4">
      <h1 class="text-primary fw-bold">Brand toolkit</h1>
      <p class="text-muted fw-bold my-2 lh-base">
        We have clear guidelines for using our logo, colors, and typography. See
        below for details.
      </p>
    </header>
    <main class="container px-4 py-2 my-4 py-md-5 my-md-2">
      <div class="card mb-3">
        <div class="card-header">
          <h5 class="fw-bold text-primary">Multividas Brand</h5>
        </div>
        <div class="card-body">
          <div
            class="d-md-flex justify-content-between align-items-center gap-5 p-3"
          >
            <div
              class="d-md-flex justify-content-start align-items-center gap-5"
            >
              <div>
                <g-image
                  alt="multividas, multividas api documentation, multividas threads, multividas status, multividas help center, multividas developer, multividas about us, multividas ads, multividas engineering blog, multividas developers documentation, multividas embed threadsmultividas, multividas api documentation, multividas threads, multividas status, multividas help center, multividas developer, multividas about us, multividas ads, multividas engineering blog, multividas developers documentation, multividas embed threadsmultividas, multividas api documentation, multividas threads, multividas status, multividas help center, multividas developer, multividas about us, multividas ads, multividas engineering blog, multividas developers documentation, multividas embed threadsmultividas, multividas api documentation, multividas threads, multividas status, multividas help center, multividas developer, multividas about us, multividas ads, multividas engineering blog, multividas developers documentation, multividas"
                  src="~/assets/png/nav-multividas-blogging-platform-multividas-social-media-blog-multividas-posts-threads-multividas-comments-discussions-multividas-short-texts-multividas-social-blogging.svg"
                  width="150"
                  height="150"
                  class="mb-3 mb-md-0"
                />
              </div>
              <div>
                <h2 class="mb-3 mb-md-0">Multividas logo</h2>
                <p class="mb-3 mb-md-0">
                  Our logo is our most recognizable asset, and we hold it in
                  high regard. Please take a moment to consider the manner in
                  which you utilize it.
                </p>
              </div>
            </div>
            <div>
              <a
                class="btn btn-sm btn-light border text-xxs fw-medium px-3 py-2 rounded-4"
                href="https://about.multividas.com/assets/static/multividas-logo.zip"
                target="_blank"
                download
              >
                Download
              </a>
            </div>
          </div>

          <hr />

          <div class="p-3">
            <h5 class="mb-2">Multividas Logo</h5>
            <p>
              Primary color
              <span class="fw-bold text-primary fs-5 mx-2">#0f4c81</span>
            </p>
            <p>
              Typography font
              <span class="fw-bold text-primary fs-5 mx-2">Multividas</span>
            </p>
          </div>

          <hr />

          <div class="p-3">
            <h5 class="mb-2">Legal disclaimer</h5>
            <p class="mb-2">
              By using the Multividas trademarks and resources on this site, you
              agree to follow the Multividas Trademark Guidelines in our Brand
              Guidelines — as well as our Terms of Service and all other
              Multividas rules and policies. If you have any questions, contact
              us at
              <a href="mailto:contact@multividas.com"
                ><code class="text-primary">contact@multividas.com</code></a
              >
            </p>
            <ul class="legal-notices">
              <li>
                Please don’t edit the logos when using them. Resizing is
                permitted of course.
              </li>
              <li>
                Make sure you maintain legibility for print and digital media by
                using the right dimensions.
              </li>
            </ul>
          </div>
        </div>
      </div>
    </main>
  </MainLayout>
</template>

<script>
export default {
  metaInfo: {
    title: "Brand toolkit",
  },
};
</script>

<style>
ul.legal-notices {
  list-style-type: disc !important;
  padding-left: 25px !important;
}
</style>
