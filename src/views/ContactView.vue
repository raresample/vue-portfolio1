<template>
  <div class="about">

    <div class="container">
      <!--Section: Contact v.2-->
      <section class="mb-4">

          <!--Section heading-->
          <h2 class="h1-responsive font-weight-bold text-center my-4">Contact me</h2>
          <!--Section description-->
          <p class="text-center w-responsive mx-auto mb-5">Send me a message here and I'll get back to you soon.</p>

          <div class="row">

              <!--Grid column-->
              <div class="col-md-9 mb-md-0 mb-5">
                  <form id="contact-form" name="contact-form" action="mail.php" method="POST">

                      <!--Grid row-->
                      <div class="row">

                          <!--Grid column-->
                          <div class="col-md-6">
                              <div class="md-form mb-0">
                                  <input type="text" id="name" name="name" class="form-control">
                                  <label for="name" class="">Your name</label>
                              </div>
                          </div>
                          <!--Grid column-->

                          <!--Grid column-->
                          <div class="col-md-6">
                              <div class="md-form mb-0">
                                  <input type="text" id="email" name="email" class="form-control">
                                  <label for="email" class="">Your email</label>
                              </div>
                          </div>
                          <!--Grid column-->

                      </div>
                      <!--Grid row-->

                      <!--Grid row-->
                      <div class="row">
                          <div class="col-md-12">
                              <div class="md-form mb-0">
                                  <input type="text" id="subject" name="subject" class="form-control">
                                  <label for="subject" class="">Subject</label>
                              </div>
                          </div>
                      </div>
                      <!--Grid row-->

                      <!--Grid row-->
                      <div class="row">

                          <!--Grid column-->
                          <div class="col-md-12">

                              <div class="md-form">
                                  <textarea type="text" id="message" name="message" rows="2" class="form-control md-textarea"></textarea>
                                  <label for="message">Your message</label>
                              </div>

                          </div>
                      </div>
                      <!--Grid row-->

                  </form>

                  <div class="text-center text-md-left">
                      <!-- <a class="btn btn-primary" onclick="document.getElementById('contact-form').submit();">Send</a> -->
                      <a id="sendButton" class="btn btn-primary" onclick="document.getElementById('contact-form').submit();">Send</a>
                  </div>
                  <div class="status"></div>
              </div>
              <!--Grid column-->

              <!--Grid column-->
              <div class="col-md-3 text-center">
                  <ul class="list-unstyled mb-0">
                      <li><i class="fas fa-map-marker-alt fa-2x"></i>
                          <p>Los Angeles, CA 90014, USA</p>
                      </li>

                      <li><i class="fas fa-phone mt-4 fa-2x"></i>
                          <p>530.601.1500</p>
                      </li>

                      <li><i class="fas fa-envelope mt-4 fa-2x"></i>
                          <p>aghopecode@gmail.com</p>
                      </li>
                  </ul>
              </div>
              <!--Grid column-->

          </div>

      </section>
      <!--Section: Contact v.2-->
    </div>

  </div>
</template>

<style>
a#sendButton {
  background-image: linear-gradient(
    to left, rgba(78, 217, 217, 0.761) 0%,
    rgb(128, 155, 217) 100%
  );
  font-weight: bold;
}

</style>