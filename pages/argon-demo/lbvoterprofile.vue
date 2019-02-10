<template>
  <div class="profile-page">
    <modal :show.sync="modal0">
      <template slot="header">
        <h5 class="modal-title" id="contactModalLabel">Voice Call to Lena</h5>
      </template>
      <div>
        Voice Mail ....</p>
        Vote Yes on this Agenda Item 999999
      </div>
      <template slot="footer">
        <base-button type="secondary" @click="modal0 = false">Close</base-button>
      </template>
    </modal>

    <modal :show.sync="modal1">
      <template slot="header">
        <h5 class="modal-title" id="contactModalLabel">TEXT Lena</h5>
      </template>
      <div>
        TEXT.....</p>
        Vote Yes on this Agenda Item 999999
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
                    <img v-lazy="'/argon/img/theme/votelongbeachapp.png'" class="rounded-circle">
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
                    <span class="description">Surveys</span>
                  </div>
                  <div>
                    <span class="heading">10</span>
                    <span class="description">Yes</span>
                  </div>
                  <div>
                    <span class="heading">89</span>
                    <span class="description">Comments</span>
                  </div>
                </div>
              </div>
            </div>

            <tabs fill class="flex-column flex-md-row">
              <card shadow>
                <tab-pane>
                  <span slot="title">
                    <i class="ni ni-cloud-upload-96"></i>
                    Surveys
                  </span>
                  <p class="description">
                    Raw denim you probably haven't heard of them jean shorts
                    Austin. Nesciunt tofu stumptown aliqua, retro synth master cleanse. Mustache
                    cliche tempor, williamsburg carles vegan helvetica. Reprehenderit butcher retro
                    keffiyeh dreamcatcher synth.
                  </p>
                </tab-pane>
                <tab-pane title="Profile">
                  <span slot="title">
                    <i class="ni ni-bell-55 mr-2"/>
                    Council Meetings Feed
                  </span>
                  <p class="description"></p>
                  <div class="site-branding">
                    <div class="site-branding-logo">
                      <video
                        width="450"
                        controls
                        src="http://archive-media.granicus.com:443/OnDemand/longbeach/longbeach_aba09037-851c-4acf-8222-34cb1e20b23f.mp4"
                      ></video>
                    </div>
                  </div>
                  <div class="site-branding-text">
                    <div class="card-profile-image">
                      <h2>Distric #1</h2>
                      <h2>Lena Gonzalez</h2>
                    </div>
                    <div sytle="vertical-align:bottom">
                      <img
                        v-lazy="'/argon/img/theme/gonzalez185x200_dist1.jpg'"
                        class="rounded-circle"
                      >
                    </div>
                  </div>
                </tab-pane>
                <tab-pane>
                  <span slot="title">
                    <i class="ni ni-calendar-grid-58"/>
                    Events
                  </span>
                  <p class="description"></p>
                </tab-pane>
              </card>
            </tabs>
          </div>
        </card>
      </div>
    </section>
  </div>
</template>
<script>
import BaseNav from '~/components/argon/BaseNav'
import Tabs from '~/components/argon/Tabs/Tabs'
import TabPane from '~/components/argon/Tabs/TabPane'
import Tab from '~/components/argon/Tabs/Tab'
import TabsLayout from '~/components/argon/Tabs/TabsLayout'
import PillsLayout from '~/components/argon/Tabs/PillsLayout'
import Modal from '~/components/argon/Modal'

export default {
  layout: 'argon-demo',
  components: {
    Tabs,
    TabPane,
    Tab,
    TabsLayout,
    BaseNav,
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
<style scoped>
div.site-branding {
  /* Position Logo and Text  */
  display: inline;
  /* vertical-align: middle; */
}

div.site-branding-logo {
  /* Position logo within site-branding */
  display: inline-block;
  vertical-align: middle;
}

div.site-branding-text {
  /* Position text within site-branding */
  display: inline-block;
  width: 350px;
  margin: auto 0;
  vertical-align: top;
}
div.site-branding-text-logo {
  /* Position text within site-branding */
  display: inline-block;
  margin: auto 0;
  vertical-align: bottom;
}

div.site-branding-title {
  /* Position title within text */
  display: inline-block;
}

div.site-branding-tagline {
  /* Position tagline within text */
  display: inline-block;
}
</style>