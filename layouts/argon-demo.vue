<template>
  <div>
    <header class="header-global">
      <base-nav class="navbar-main" transparent type effect="light" expand>
        <nuxt-link slot="brand" class="navbar-brand mr-lg-5" :to="{name: 'argon-demo-landing'}">
          <img height="600" width="101" src="/argon/img/brand/actlblogoiii.png">
        </nuxt-link>

        <ul class="navbar-nav navbar-nav-hover align-items-lg-center">
          <li class="nav-item nav-link-inner--text">
            <nuxt-link :to="{name: 'argon-demo-landing'}">Home</nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link :to="{name: 'argon-demo-register'}">Register</nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link :to="{name: 'argon-demo-login'}">Login</nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link :to="{name: 'argon-demo-aboutus'}">About Us</nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link :to="{name: 'argon-demo-contact'}">Contact</nuxt-link>
          </li>
        </ul>

        <ul class="navbar-nav align-items-lg-center ml-lg-auto">
          <li class="nav-item">
            <a
              class="nav-link nav-link-icon"
              href="https://www.facebook.com/actlb"
              target="_blank"
              data-toggle="tooltip"
              title="Like us on Facebook"
            >
              <i class="fa fa-facebook-square"></i>
              <span class="nav-link-inner--text d-lg-none">Facebook</span>
            </a>
          </li>
          <li class="nav-item">
            <a
              class="nav-link nav-link-icon"
              href="https://www.instagram.com/actlbofficial"
              target="_blank"
              data-toggle="tooltip"
              title="Follow us on Instagram"
            >
              <i class="fa fa-instagram"></i>
              <span class="nav-link-inner--text d-lg-none">Instagram</span>
            </a>
          </li>
          <li class="nav-item">
            <a
              class="nav-link nav-link-icon"
              href="https://twitter.com/actlb"
              target="_blank"
              data-toggle="tooltip"
              title="Follow us on Twitter"
            >
              <i class="fa fa-twitter-square"></i>
              <span class="nav-link-inner--text d-lg-none">Twitter</span>
            </a>
          </li>
          <li class="nav-item">
            <a
              class="nav-link nav-link-icon"
              href="https://github.com/theownerofactname"
              target="_blank"
              data-toggle="tooltip"
              title="Star us on Github"
            >
              <i class="fa fa-github"></i>
              <span class="nav-link-inner--text d-lg-none">Github</span>
            </a>
          </li>
          <li class="nav-item d-none d-lg-block ml-lg-4">
            <!--
            <a
              href="https://www.creative-tim.com/product/vue-argon-design-system"
              target="_blank"
              class="btn btn-neutral btn-icon"
            >
              <span class="btn-inner--icon">
                <i class="fa fa-cloud-download mr-2"></i>
              </span>
              <span class="nav-link-inner--text">Download</span>
            </a>
            -->
          </li>
        </ul>
      </base-nav>
    </header>
    <main>
      <nuxt/>
    </main>
    <footer class="footer has-cards">
      <!--
      <div class="container container-lg">
        <div class="row">
          <div class="col-md-6 mb-5 mb-md-0">
            <div class="card card-lift--hover shadow border-0">
              <nuxt-link :to="{name: 'argon-demo-landing'}" title="Landing Page">
                <img v-lazy="'/argon/img/theme/landing.jpgx'" class="card-img">
              </nuxt-link>
            </div>
          </div>
          <div class="col-md-6 mb-5 mb-lg-0">
            <div class="card card-lift--hover shadow border-0">
              <nuxt-link :to="{name: 'argon-demo-profile'}" title="Profile Page">
                <img v-lazy="'/argon/img/theme/profile.jpgx'" class="card-img">
              </nuxt-link>
            </div>
          </div>
        </div>
      </div>
      -->
      <div class="container">
        <div class="row row-grid align-items-center my-md">
          <div class="col-lg-6">
            <h3 class="text-primary font-weight-light mb-2">Thank you for supporting us!</h3>
            <h4 class="mb-0 font-weight-light">Let's get in touch on any of these platforms.</h4>
          </div>
          <div class="col-lg-6 text-lg-center btn-wrapper">
            <a
              target="_blank"
              href="https://twitter.com/actlb"
              class="btn btn-neutral btn-icon-only btn-twitter btn-round btn-lg"
              data-toggle="tooltip"
              data-original-title="Follow us"
            >
              <i class="fa fa-twitter"></i>
            </a>
            <a
              target="_blank"
              href="https://www.facebook.com/actlb"
              class="btn btn-neutral btn-icon-only btn-facebook btn-round btn-lg"
              data-toggle="tooltip"
              data-original-title="Like us"
            >
              <i class="fa fa-facebook-square"></i>
            </a>
            <a
              target="_blank"
              href="https://dribbble.com/actlb"
              class="btn btn-neutral btn-icon-only btn-dribbble btn-lg btn-round"
              data-toggle="tooltip"
              data-original-title="Follow us"
            >
              <i class="fa fa-dribbble"></i>
            </a>
            <a
              target="_blank"
              href="https://github.com/theownerofactname"
              class="btn btn-neutral btn-icon-only btn-github btn-round btn-lg"
              data-toggle="tooltip"
              data-original-title="Star on Github"
            >
              <i class="fa fa-github"></i>
            </a>
          </div>
        </div>
        <hr>
        <div class="row align-items-center justify-content-md-between">
          <div class="col-md-6">
            <div class="copyright">
              &copy; 2018
              <a href="#" target="#">ACT Long Beach</a>.
            </div>
          </div>
          <div class="col-md-6">
            <ul class="nav nav-footer justify-content-end">
              <li class="nav-item">
                <a href="#" class="nav-link" target="#">Act Long Beach</a>
              </li>
              <li class="nav-item">
                <a href="#" class="nav-link" target="#">
                  About
                  Us
                </a>
              </li>
              <li class="nav-item">
                <a href="http://blog.ownerofactname" class="nav-link" target="_blank">Blog</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import BaseNav from '~/components/argon/BaseNav'
import BaseDropdown from '~/components/argon/BaseDropdown'
import CloseButton from '~/components/argon/CloseButton'

export default {
  components: {
    BaseNav,
    CloseButton,
    BaseDropdown
  }
}
</script>

<style>
nav .navbar-nav li a {
  color: white !important;
}
</style>
