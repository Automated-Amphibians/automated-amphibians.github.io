---
layout: front-page
title: 
description: FRC Team 8426, Automated Amphibians.
keywords: frc, automated amphibians, robotics
---

<style>
    li.nav-item {
        margin-left: 2.5em;
    }

    .content {
        margin-top: 2em;
        font-size: 110%;
    }

    .carousel-control-next,
    .carousel-control-prev {
        width: initial;
        background: #888;

    }

    .carousel-item {
        padding: 2em;
    }
</style>

[The Automated Amphibians](about) are a [FIRST FRC](https://www.firstinspires.org/robotics/frc) team based out of Novi High School. 

Automated Amphibians is proud to announce it has qualified for a trip to FRC Worlds Competition! See you in Houston!

<div style="position: relative; width: 800px; height: 600px;">
  <img src="assets/team-latest.jpg" style="position: absolute; width: 100%; height: 100%; opacity: 1; transition: opacity 1s ease-in-out;" id="image1"/>  
  <img src="assets/Robotplacingcone.jpg" style="position: absolute; width: 100%; height: 100%; opacity: 0; transition: opacity 1s ease-in-out;" id="image3"/>
</div>

<script>
var images = [document.getElementById('image1'), document.getElementById('image3')];
var current = 0;

function nextImage() {
  images[current].style.opacity = 0;
  current = (current + 1) % images.length;
  images[current].style.opacity = 1;
}
setInterval(nextImage, 5000); // change image every 5 seconds
</script>



{% comment %} 

Sidebar can be for latest stuff?
Carousel is for highlighted/important stuff

MVP:
    What we're building, goals
    About (contact)
    Tools/Our partners and sponsors
    Previous year (robots)       
    Things we've published (blog, video?) 

{% endcomment %} 
