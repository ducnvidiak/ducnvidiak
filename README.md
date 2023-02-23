<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
      /* Main styles */
      @import url(https://fonts.googleapis.com/css?family=Open+Sans:800);
      .text {
        fill: none;
        stroke-width: 3;
        stroke-linejoin: round;
        stroke-dasharray: 70 330;
        stroke-dashoffset: 0;
        -webkit-animation: stroke 6s infinite linear;
        animation: stroke 6s infinite linear;
      }
      .text:nth-child(5n + 1) {
        stroke: #f2385a;
        -webkit-animation-delay: -1.2s;
        animation-delay: -1.2s;
      }
      .text:nth-child(5n + 2) {
        stroke: #f5a503;
        -webkit-animation-delay: -2.4s;
        animation-delay: -2.4s;
      }
      .text:nth-child(5n + 3) {
        stroke: #e9f1df;
        -webkit-animation-delay: -3.6s;
        animation-delay: -3.6s;
      }
      .text:nth-child(5n + 4) {
        stroke: #56d9cd;
        -webkit-animation-delay: -4.8s;
        animation-delay: -4.8s;
      }
      .text:nth-child(5n + 5) {
        stroke: #3aa1bf;
        -webkit-animation-delay: -6s;
        animation-delay: -6s;
      }

      @-webkit-keyframes stroke {
        100% {
          stroke-dashoffset: -400;
        }
      }
      @keyframes stroke {
        100% {
          stroke-dashoffset: -400;
        }
      }
      /* Other styles */
      html,
      body {
        height: 100%;
      }

      body {
        background: #111;
        background-size: 0.2em 100%;
        font: 5em/1 Open Sans, Impact;
        text-transform: uppercase;
        margin: 0;
      }

      svg {
        position: absolute;
        width: 100%;
        height: 100%;
      }
    </style>
  </head>
  <body>
    <svg viewBox="0 0 600 300">
      <!-- Symbol-->
      <symbol id="s-text">
        <text text-anchor="middle" x="50%" y="50%" dy=".35em">
          ducit488
        </text>
      </symbol>
      <!-- Duplicate symbols-->
      <use class="text" xlink:href="#s-text"></use>
      <use class="text" xlink:href="#s-text"></use>
      <use class="text" xlink:href="#s-text"></use>
      <use class="text" xlink:href="#s-text"></use>
      <use class="text" xlink:href="#s-text"></use>
    </svg>
  </body>
</html>
