<template>
  <div class="profile-page">
    <section class="section-profile-cover section-shaped my-0">
      <div class="shape shape-style-1 shape-primary shape-skew alpha-4">
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
      </div>
    </section>
    <section class="section section-skew">
      <div class="container">
        <card shadow class="card-profile mt--400" no-body>
          <div class="px-4">
            <div class="row justify-content-center">
              <div class="col-lg-3 order-lg-2">
                <div class="card-profile-image">
                  <a href="#">
                    <img
                      v-lazy="'/argon/img/theme/gonzalez185x200_dist1x.jpg'"
                      class="rounded-circle"
                    >
                  </a>
                </div>
              </div>Contact Us
              <div class="col-lg-4 order-lg-3 text-lg-right align-self-lg-center">
                <div class="card-profile-actions py-4 mt-lg-0">
                  <base-button type="info" size="sm" class="mr-4" @click="modal0 = true">Connect</base-button>
                  <base-button
                    type="default"
                    size="sm"
                    class="float-right"
                    @click="modal1 = true"
                  >Message</base-button>
                </div>
              </div>
              <div class="col-lg-4 order-lg-1"></div>
            </div>

            <!--
            <div class="mt-5 py-5 border-top text-center">
              <div class="row justify-content-center">
                <div class="col-lg-9">
                  <p>An artist of considerable range, Ryan — the name taken by Melbourne-raised, Brooklyn-based Nick Murphy — writes, performs and records all of his own music, giving it a warm, intimate feel with a solid groove structure. An artist of considerable range.</p>
                  <a href="#">Show more</a>
                </div>
              </div>
            </div>
            -->
          </div>
        </card>
      </div>
    </section>
  </div>
</template>
<script>
import Modal from '~/components/argon/Modal'

export default {
  layout: 'argon-demo',
  components: {
    Modal
  },
  data() {
    return {
      modal0: false,
      modal1: false
    }
  }
}
</script>
<style>
</style>
