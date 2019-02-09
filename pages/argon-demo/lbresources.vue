<template>
  <div class="profile-page">
    <section class="section-profile-cover section-shaped my-0">
      <div class="shape shape-style-1 shape-primary shape-skew alpha-4">
        <span></span>
        <span></span>
      </div>
    </section>
    <section class="section section-skew">
      <div class="container">
        <card shadow class="card-body mt--400" no-body>
          <style>
            .embed-container {
              position: relative;
              padding-bottom: 80%;
              height: 0;
              max-width: 100%;
            }
            .embed-container iframe,
            .embed-container object,
            .embed-container iframe {
              position: absolute;
              top: 0;
              left: 0;
              width: 100%;
              height: 100%;
            }
            small {
              position: absolute;
              z-index: 40;
              bottom: 0;
              margin-bottom: -15px;
            }
          </style>
          <div class="embed-container">
            <small>
              <a
                href="//www.arcgis.com/apps/Embed/index.html?webmap=2ff8e7f59c9b470f8397eeeed0fda045&extent=-118.3418,33.7248,-117.9566,33.872&home=true&zoom=true&scale=true&search=true&searchextent=true&details=true&legendlayers=true&active_panel=legend&basemap_gallery=true&disable_scroll=false&theme=light"
                style="color:#0000FF;text-align:left"
                target="_blank"
              >View larger map</a>
            </small>
            <br>
            <iframe
              width="500"
              height="400"
              frameborder="0"
              scrolling="no"
              marginheight="0"
              marginwidth="0"
              title="MapIt Service Locations (Public Web Map)"
              src="//www.arcgis.com/apps/Embed/index.html?webmap=2ff8e7f59c9b470f8397eeeed0fda045&extent=-118.3418,33.7248,-117.9566,33.872&home=true&zoom=true&previewImage=false&scale=true&search=true&searchextent=true&details=true&legendlayers=true&active_panel=legend&basemap_gallery=true&disable_scroll=false&theme=light"
            ></iframe>
          </div>

          <div class="px-4">
            <!--  
            <div class="row justify-content-center">
              <div class="col-lg-3 order-lg-2">
                <div class="card-profile-image">
                  <a href="#">
                    <img v-lazy="'/argon/img/theme/team-4-800x800.jpg'" class="rounded-circle">
                  </a>
                </div>
              </div>
              
              <div class="col-lg-4 order-lg-3 text-lg-right align-self-lg-center">
                <div class="card-profile-actions py-4 mt-lg-0">
                  <base-button type="info" size="sm" class="mr-4">Connect</base-button>
                  <base-button type="default" size="sm" class="float-right">Message</base-button>
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
            -->
            <div class="mt-5 py-5 border-top text-center">
              <div class="row justify-content-center">
                <div class="col-lg-9"></div>
              </div>
            </div>
          </div>
        </card>
      </div>
    </section>
  </div>
</template>
<script>
export default {
  layout: 'argon-demo'
}
</script>
<style>
</style>