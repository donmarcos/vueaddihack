<template>
  <div>
    <div class="position-relative">
      <!-- shape Hero -->
      <video-bg :sources="['/argon/img/theme/back.mp4']" img>
        <section class="section-shaped my-0">
          <div class="shape shape-style-1 shape-default shape-skew">
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
          </div>
          <div class="container shape-container d-flex">
            <div class="col px-0">
              <div class="row">
                <div class="col-lg-6">
                  <h1 class="display-3 text-white">
                    ACT Long Beach
                    <span></span>
                  </h1>
                  <p class="lead text-white">Take action and make your elected official accountable</p>
                  <div class="btn-wrapper">
                    <nuxt-link :to="{name: 'argon-demo-register'}">
                      <base-button
                        tag="a"
                        class="mb-3 mb-sm-0"
                        type="info"
                        icon="fa fa-code"
                      >Join Us</base-button>
                    </nuxt-link>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>
      </video-bg>

      <!-- 1st Hero Variation -->
    </div>
    <section class="section section-lg pt-lg-0 mt--200">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-lg-12">
            <div class="row row-grid">
              <div class="col-lg-4">
                <card class="border-0" hover shadow body-classes="py-5">
                  <icon name="ni ni-check-bold" type="primary" rounded class="mb-4"></icon>
                  <h6 class="text-primary text-uppercase">Districts</h6>
                  <p class="description mt-3">
                    Long Beach has several districts
                    where are you located ?
                    Find out
                  </p>
                  <div>
                    <badge type="primary" rounded>Location</badge>
                    <badge type="primary" rounded>Residents</badge>
                    <badge type="primary" rounded>Boundaries</badge>
                  </div>
                  <nuxt-link :to="{name: 'argon-demo-lbdisctricts'}">
                    <base-button type="primary" class="mt-4">Discticts</base-button>
                  </nuxt-link>
                </card>
              </div>
              <div class="col-lg-4">
                <card class="border-0" hover shadow body-classes="py-5">
                  <icon name="ni ni-istanbul" type="success" rounded class="mb-4"></icon>
                  <h6 class="text-success text-uppercase">Elected Officials</h6>
                  <p class="description mt-3">
                    Want to know who is your elected representative in Long Beach ?
                    Let's find out
                  </p>
                  <div>
                    <badge type="success" rounded>Goverment</badge>
                    <badge type="success" rounded>vision</badge>
                    <badge type="success" rounded>info</badge>
                  </div>
                  <nuxt-link :to="{name: 'argon-demo-lbelected'}">
                    <base-button type="success" class="mt-4">Learn more</base-button>
                  </nuxt-link>
                </card>
              </div>
              <div class="col-lg-4">
                <card class="border-0" hover shadow body-classes="py-5">
                  <icon name="ni ni-planet" type="warning" rounded class="mb-4"></icon>
                  <h6 class="text-warning text-uppercase">Resources</h6>
                  <p class="description mt-3">
                    Long Beach has multiple resources for its residents
                    check the interactive map
                  </p>
                  <div>
                    <badge type="warning" rounded>marketing</badge>
                    <badge type="warning" rounded>product</badge>
                    <badge type="warning" rounded>Business</badge>
                  </div>
                  <nuxt-link :to="{name: 'argon-demo-lbresources'}">
                    <base-button type="warning" class="mt-4">Learn more</base-button>
                  </nuxt-link>
                </card>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'home',
  layout: 'argon-demo',
  components: {}
}
</script>
