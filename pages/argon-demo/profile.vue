<template>
  <div class="profile-page">
    <modal :show.sync="modal0">
      <template slot="header">
        <h5 class="modal-title" id="contactModalLabel">Voice Call to Lena</h5>
      </template>
      <div>Voice Mail ....
        <p></p>Vote Yes on this Agenda Item 999999
      </div>
      <template slot="footer">
        <base-button type="secondary" @click="modal0 = false">Close</base-button>
      </template>
    </modal>

    <modal :show.sync="modal1">
      <template slot="header">
        <h5 class="modal-title" id="contactModalLabel">TEXT Lena</h5>
      </template>
      <div>TEXT.....
        <p></p>Vote Yes on this Agenda Item 999999
      </div>
      <template slot="footer">
        <base-button type="secondary" @click="modal1 = false">Close</base-button>
      </template>
    </modal>

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
        <card shadow class="card-profile mt--450" no-body>
          <div class="px-4">
            <div class="row justify-content-center">
              <div class="col-lg-3 order-lg-2">
                <div class="card-profile-image">
                  <a href="#">
                    <img
                      v-lazy="'/argon/img/theme/gonzalez185x200_dist1.jpg'"
                      class="rounded-circle"
                    >
                  </a>
                </div>
              </div>
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
              <div class="col-lg-4 order-lg-1">
                <div class="card-profile-stats d-flex justify-content-center">
                  <div>
                    <span class="heading">22</span>
                    <span class="description">Friends</span>
                  </div>
                  <div>
                    <span class="heading">10</span>
                    <span class="description">Photos</span>
                  </div>
                  <div>
                    <span class="heading">89</span>
                    <span class="description">Comments</span>
                  </div>
                </div>
              </div>
            </div>
            <div class="text-center mt-5">
              <h3>
                Jessica Jones
                <span class="font-weight-light">, 27</span>
              </h3>
              <div class="h6 font-weight-300">
                <i class="ni location_pin mr-2"></i>Bucharest, Romania
              </div>
              <div class="h6 mt-4">
                <i class="ni business_briefcase-24 mr-2"></i>Solution Manager - Creative Tim Officer
              </div>
              <div>
                <i class="ni education_hat mr-2"></i>University of Computer Science
              </div>
            </div>
            <div class="mt-5 py-5 border-top text-center">
              <div class="row justify-content-center">
                <div class="col-lg-9">
                  <p>An artist of considerable range, Ryan — the name taken by Melbourne-raised, Brooklyn-based Nick Murphy — writes, performs and records all of his own music, giving it a warm, intimate feel with a solid groove structure. An artist of considerable range.</p>
                  <a href="#">Show more</a>
                </div>
              </div>
            </div>
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
