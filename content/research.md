---
title: ""
draft: false
---

## Research projects

Visit Qixuan Chen's [Google Scholar profile](http://scholar.google.com/citations?user=gHLwOp4AAAAJ&hl=en&oi=ao).

A full cv file can be found [here](/files/2026_01_CV_CHEN.pdf).

<style>

.overlay-grid{
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 28px;
  margin-top: 36px;
  overflow: visible;  
}

.overlay-card{
  position: relative;
  height: 340px;
  border-radius: 12px;
  overflow: visible;
  transition: transform .35s ease, box-shadow .35s ease, opacity .35s ease;
  z-index: 0;
}

.overlay-card:hover{
  transform: scale(1.08) translateY(-6px);
  z-index: 20;
  box-shadow: 0 25px 60px rgba(0,0,0,0.35);
}

.overlay-card .bg{
  position: absolute;
  inset: 0;
  background-size: cover;
  background-position: center;
  transition: transform .6s ease;
}

.overlay-card:hover .bg{
  transform: scale(1.05);
}


.overlay-card .box{
  position: absolute;
  bottom: 16px;
  right: 16px;
  width: min(70%, 360px);
  background: rgba(255,255,255,0.96);
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 12px 28px rgba(0,0,0,0.18);
}

.overlay-card .box h3{
  margin: 0 0 8px 0;
  font-size: 26px;
}

.overlay-card .box p{
  margin: 0 0 12px 0;
  line-height: 1.55;
}

.overlay-card .btn,
.overlay-card .btn:link,
.overlay-card .btn:visited{
  display: inline-block;
  padding: 6px 0;
  border: none;
  background: transparent;
  text-decoration: none;
  color: #fff !important;
  font-weight: 600;
  font-size: 15px;
}

.overlay-card .btn:hover,
.overlay-card .btn:active{
  color: #fff !important;
  text-decoration: none;
}


@media (max-width: 900px){
  .overlay-grid{
    grid-template-columns: 1fr;
  }

  .overlay-card .box{
    left: 50%;
    right: auto;
    transform: translateX(-50%);
    width: 85%;
  }
}


.hover-content{
  opacity: 0;
  transform: translateY(12px);
  max-height: 0;
  overflow: hidden;
  transition: all 0.4s ease;
}


.overlay-card:hover .hover-content{
  opacity: 1;
  transform: translateY(0);
  max-height: 200px;
  margin-top: 10px;
}


.overlay-card:hover .bg{
  transform: scale(1.08);
}



.overlay-card:hover .hover-desc{
  opacity: 1;
  transform: translateY(0);
}


.overlay-card:hover .bg{
  transform: scale(1.08);
}


.overlay-card.card-survey .box{
  background: rgba(255,255,255,0);  
  box-shadow: none;                
  backdrop-filter: none;         
}
.overlay-card.card-survey .box h3{
  color: #fff;
  text-shadow: 0 2px 10px rgba(0,0,0,.35);
}


.overlay-grid:hover .overlay-card{
  opacity: 0.45;
  filter: saturate(0.75) brightness(1.05);
  transform: none; 
}


.overlay-grid:hover .overlay-card:hover{
  opacity: 1;
  filter: none;
  transform: scale(1.08) translateY(-6px);
}

</style>

<div class="overlay-grid">

  <div class="overlay-card card-survey">
    <div class="bg" style="background-image:url('/images/research/survey.png');"></div>
    <div class="box">
      <h3>Bayesian Survey Inference</h3>
      <div class="hover-content">
        <a class="btn" href="/project/survey_inference/">Read More</a>
      </div>
    </div>
  </div>


  <div class="overlay-card card-survey">
    <div class="bg" style="background-image:url('/images/research/generalizability.png');"></div>
    <div class="box">
      <h3>Health Survey Application</h3>
      <div class="hover-content">
        <a class="btn" href="/project/health_app/">Read More</a>
      </div>
    </div>
  </div>

  <div class="overlay-card card-survey">
    <div class="bg" style="background-image:url('/images/research/measurement.jpg');"></div>
    <div class="box">
      <h3>Measurement Error</h3>
      <div class="hover-content">
        <a class="btn" href="/project/measurement_error/">Read More</a>
      </div>
    </div>
  </div>

  <div class="overlay-card card-survey">
    <div class="bg" style="background-image:url('/images/research/missing.png');"></div>
    <div class="box">
      <h3>Missing Data</h3>
      <div class="hover-content">
        <a class="btn" href="../project/missing_data/">Read More</a>
      </div>
    </div>
  </div>

  <div class="overlay-card card-survey">
    <div class="bg" style="background-image:url('/images/research/epidemiological.jpg');"></div>
    <div class="box">
      <h3>Epidemiological Research</h3>
      <div class="hover-content">
        <a class="btn" href="/project/epi_research/">Read More</a>
      </div>
    </div>
  </div>
  
  <!--
  <div class="overlay-card card-survey">
    <div class="bg" style="background-image:url('/images/research/fall.png');"></div>
    <div class="box">
      <h3>Survey Design</h3>
      <div class="hover-content">
        <a class="btn" href="/project/survey_design/">Read More</a>
      </div>
    </div>
  </div>
  -->

</div>
