<!DOCTYPE html>
<html lang="en-us">
 
  <head>
    <meta charset="utf-8" />
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
    <meta
      name="viewport"
      content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=0"
    />
    <title>Opticwear AR</title>
    <link rel="stylesheet" href="style.css" />
  </head>

  <body>
 

    <!-- loading screen -->
    <div class="fixed-fullscreen" id="loading-screen">
      <div
        style="
          display: flex;
          flex-direction: column;
          align-items: center;
          justify-content: center;
        "
      >
        <img
          id="initial-loading-logo"
          style="max-width: 200px"
          src="./thumbs/opticwear-world.png"
          class=""
        />
        <div
          style="
            width: 100%;
            height: 8px;
            margin-top: 20px;
            background-color: rgb(55 65 81 / 1);
            border-radius: 100px;
            overflow: hidden;
          "
        >
          <div id="loading-progress-bar"></div>
        </div>
       <p style="color:white">Loading Opticwear Ar Try-On...</p>
      </div>
    </div>

    <!-- permission denied screen -->
    <div
      class="fixed-fullscreen screen"
      id="permission-denied-screen"
      style="display: none"
    >
      <div class="permission-denied-text-container">
        <div class="permission-denied-text" id="camera_denied">
          <p>Oops! Please reload and allow camera access to use Opticwear AR.</p>
          <a
            class="permission-denied-button"
            href="https://www.opticwear.co/shop"
            target="__blank"
          >
            Back to Site
          </a>
        </div>
      </div>
    </div>

    <!-- AR screen -->
    <div class="fixed-fullscreen screen" id="ar-screen" style="display: none">
      <!-- <canvas class="deepar" id="deepar-canvas"></canvas> -->

      <div class="carousel" id="carousel">
        <div class="carousel-center" id="carousel-center">
          <div class="lds-ring" id="loading-spinner" style="display: none">
            <div></div>
            <div></div>
            <div></div>
            <div></div>
          </div>
        </div>
        <div class="carousel-slider">
          <div class="slide">
            <img class="responsive-img" src="thumbs/ray-ban-wayfarer.png" />
          </div>
          <div class="slide">
            <img class="responsive-img" src="thumbs/opticwear-world.png" />
          </div>
        </div>
      </div>
    </div>
    
    <script type="text/javascript" src="main.js"></script>
  </body>
</html>
