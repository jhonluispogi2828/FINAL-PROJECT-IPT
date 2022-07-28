# FINAL-PROJECT-IPT
<!DOCTYPE html>
<html lang="en">

  <head>

    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
    <meta name="description" content="">
    <link href="https://fonts.googleapis.com/css?family=Poppins:100,200,300,400,500,600,700,800,900" rel="stylesheet">

    <title>My Final Project in IPT</title>

    <!-- Bootstrap core CSS -->
    <link href="vendor/bootstrap/css/bootstrap.min.css" rel="stylesheet">


    <!-- Additional CSS Files -->
    <link rel="stylesheet" href="assets/css/fontawesome.css">
    <link rel="stylesheet" href="assets/css/templatemo-edu-meeting.css">
    <link rel="stylesheet" href="assets/css/owl.css">
    <link rel="stylesheet" href="assets/css/lightbox.css">

  </head>

<body>

  <!-- Sub Header -->
  <div class="sub-header">
    <div class="container">
      <div class="row">
        <div class="col-lg-8 col-sm-8">
          <div class="left-content">
           
          </div>
        </div>
        <div class="col-lg-4 col-sm-4">
          <div class="right-icons">
            <ul>
              <li><a href="https://www.facebook.com/jhonluis.flores"><i class="fa fa-facebook"></i></a></li>
              <li><a href="https://instagram.com/luisluisluisxd"><i class="fa fa-instagram"></i></a></li>
             
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- ***** Header Area Start ***** -->
  <header class="header-area header-sticky">
      <div class="container">
          <div class="row">
              <div class="col-12">
                  <nav class="main-nav">
                      <!-- ***** Logo Start ***** -->
                      <a href="index.html" class="logo">
                         FINAL PROJECT IN IPT
                      </a>
                      <!-- ***** Logo End ***** -->
                      <!-- ***** Menu Start ***** -->
                      <ul class="nav">
                          <li class="scroll-to-section"><a href="#top" class="active">ACTIVITIES</a></li>
                          <li><a href="act2/act2.html">ACTIVITY 2</a></li>
                          <li><a href="act3/act3.html">ACTIVITY 3</a></li>
                          <li><a href="act4/act4.html">ACTIVITY 4</a></li>
                          <li><a href="act5/act5.html">ACTIVITY 5</a></li>
    
                      </a>
                     
                  </nav>
              </div>  
          </div>
      </div>
  </header>
  
  <section class="section main-banner" id="top" data-section="section1">
      <video autoplay muted loop id="bg-video">
          <source src="assets/images/xmen.mp4" type="video/mp4" />
      </video>

      <div class="video-overlay header-text">
          <div class="container">
            <div class="row">
              <div class="col-lg-12">
                <div class="caption">
              <h6>BSIT - 2G</h6>
              <h2>JHON LUIS C. FLORES</h2>
              <p>Its a pleasure to be your student sir Jonas Macapagal! Thankyousomuch for teaching us!.</p>
              <div class="main-button-red">
              </div>
          </div>
              </div>
            </div>
          </div>
      </div>
  </section>
  <!-- ***** Main Banner Area End ***** -->

  <section class="services">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="owl-service-item owl-carousel">
          
            <div class="item">
              <div class="icon">
                <img src="assets/images/head 3.png" alt="">
              </div>
              <div class="down-content">
                <h4 style="color: black">Activity 2</h4>
                <p  style="color: black"> CREATING MY FIRST WEBPAGE </p>
              </div>
            </div>
            
            <div class="item">
              <div class="icon">
                <img src="assets/images/head 1.jpg" alt="">
              </div>
              <div class="down-content">
                <h4 style="color: black">Activity 3</h4>
                <p style="color: black">Putting some CSS in my Web Page</p>
              </div>
            </div>
            
            <div class="item">
              <div class="icon">
                <img src="assets/images/head 2.jpg" alt="">
              </div>
              <div class="down-content">
                <h4 style="color: black">Activity 4</h4>
                <p style="color: black">Adding User/Home in my Webpage.</p>
              </div>
            </div>
            
            <div class="item">
              <div class="icon">
                <img src="assets/images/head 3.png" alt="">
              </div>
              <div class="down-content">
                <h4 style="color: black">Activity 5</h4>
                <p style="color: black">Adding my Family Details Webpage</p>
              </div>
            </div>
  </section>

  
 
    <div class="footer">
      <p style="color: black">Flores, Jhon Luis C. BSIT - 2G/ IPT - 2022. 
      </p>
    </div>
  </section>

  <!-- Scripts -->
  <!-- Bootstrap core JavaScript -->
    <script src="vendor/jquery/jquery.min.js"></script>
    <script src="vendor/bootstrap/js/bootstrap.bundle.min.js"></script>

    <script src="assets/js/isotope.min.js"></script>
    <script src="assets/js/owl-carousel.js"></script>
    <script src="assets/js/lightbox.js"></script>
    <script src="assets/js/tabs.js"></script>
    <script src="assets/js/video.js"></script>
    <script src="assets/js/slick-slider.js"></script>
    <script src="assets/js/custom.js"></script>
    <script>
        //according to loftblog tut
        $('.nav li:first').addClass('active');

        var showSection = function showSection(section, isAnimate) {
          var
          direction = section.replace(/#/, ''),
          reqSection = $('.section').filter('[data-section="' + direction + '"]'),
          reqSectionPos = reqSection.offset().top - 0;

          if (isAnimate) {
            $('body, html').animate({
              scrollTop: reqSectionPos },
            800);
          } else {
            $('body, html').scrollTop(reqSectionPos);
          }

        };

        var checkSection = function checkSection() {
          $('.section').each(function () {
            var
            $this = $(this),
            topEdge = $this.offset().top - 80,
            bottomEdge = topEdge + $this.height(),
            wScroll = $(window).scrollTop();
            if (topEdge < wScroll && bottomEdge > wScroll) {
              var
              currentId = $this.data('section'),
              reqLink = $('a').filter('[href*=\\#' + currentId + ']');
              reqLink.closest('li').addClass('active').
              siblings().removeClass('active');
            }
          });
        };

        $('.main-menu, .responsive-menu, .scroll-to-section').on('click', 'a', function (e) {
          e.preventDefault();
          showSection($(this).attr('href'), true);
        });

        $(window).scroll(function () {
          checkSection();
        });
    </script>
</body>

</body>
</html>
