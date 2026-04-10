# 


<style>
.banner-wrap{
  position: relative;
  width: 100%;
  margin: 0 0 22px 0;
  padding-bottom: 60px;  
}

.page-banner{
  width: 100%;
  height: 320px;
  background-size: cover;
  background-position: center;
  border-radius: 14px;
}

.banner-title{
  position: absolute;
  right: 28px;
  top: 328px;   
  z-index: 9;
  color: #fff;
  font-size: 2.3rem;
  font-weight: 700;
  line-height: 1.1;
  text-shadow: 0 2px 10px rgba(0,0,0,.35);
}


.page-nav .nav-btn{
  position: absolute;
  z-index: 10;
  padding: 10px 14px;
  border-radius: 10px;
  text-decoration: none;
  font-size: 14px;
  line-height: 1;
  background: transparent;
  color: #fff;
  backdrop-filter: none;
  border: none;
  transition: transform .2s ease, opacity .2s ease;
}

.page-nav .nav-btn:hover{
  transform: translateY(-2px);
  opacity: 0.8;
}


.nav-back{
  top: 338px;
  left: 18px;
}

.bottom-nav{
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 16px;
  margin-top: 40px;
  padding-top: 12px;
}

.bottom-nav-btn{
  display: inline-block;
  padding: 10px 16px;
  border-radius: 10px;
  text-decoration: none;
  font-size: 15px;
  line-height: 1;
  color: #2a7ea0;
  background: transparent;
  border: none;
  transition: transform .2s ease, opacity .2s ease;
}

.bottom-nav-btn:hover{
  transform: translateY(-2px);
  opacity: 0.8;
  text-decoration: none;
}

.project-block{
  display: flex;
  gap: 24px;
  align-items: flex-start;
  margin: 20px 0 28px;
}

.project-text{
  flex: 1 1 auto;
}

.project-image{
  flex: 0 0 320px;
  max-width: 38%;
}

.project-image img{
  width: 100%;
  height: auto;
  border-radius: 12px;
  display: block;
}

@media (max-width: 900px){
  .page-banner{
    height: 220px;
  }
  
  .bottom-nav{
    flex-direction: column;
    align-items: stretch;
  }

  .bottom-nav-btn{
    text-align: center;
  }
  
  .banner-wrap{
    padding-bottom: 80px;
  }

  .page-nav .nav-btn{
    padding: 9px 12px;
    font-size: 13px;
  }

  .project-block{
    flex-direction: column;
  }

  .project-image{
    max-width: 100%;
  }
}
</style>

<div class="banner-wrap">
  <div class="page-banner" style="background-image:url('/lab/images/research/missing.png');"></div>

  <div class="page-nav">
    <a class="nav-btn nav-back" href="/lab/research/" aria-label="Back to Research">
      ← Back
    </a>
  </div>
</div>

<div class="banner-title">Missing Data</div>

The analysis of medical and population health data is often complicated by
missing and incomplete information. My work in this area is motivated by 
real-world challeneges in medical and public health research and focus on 
developing novel statistical methods and practical approaches to address these 
issues. 

<div style="height: 20px;"></div>

<div class="project-block">
  <div class="project-text">
§ denote trainees.

<p style="color: #2f6db5; font-weight: 700; font-size: 1.2rem; margin-bottom: 0.5rem;">
Statistical Focus:
</p>
My research focuses on statistical methods for handling 
missing data and variable selection in multiply imputed data. 

  </div>
</div>

**Selected publications:**

- **Chen, Q.** and Wang, S. (2013). “Variable selection for multiply imputed data with application to dioxin exposure study”, *Statistics in Medicine*, **32**, 3646–3659.

- **Chen, Q.**, Gelman, A., Tracy, M., Norris, F., and Galea, S. (2015). “Incorporating the sampling design in weighting adjustments for panel attrition”, *Statistics in Medicine*, **34**(28), 3637–3647.

- **Chen, Q.**, Paik, M. C., Kim, M., and Wang, C. (2016). “Using link-preserving imputation for logistic partially linear models with missing covariates”, *Computational Statistics and Data Analysis*, **101**, 174–185.

- Zou, J.§, Wang, S., and **Chen, Q.** “Bayesian MI-LASSO for variable selection on multiply imputed data”, submitted.

<div style="height: 20px;"></div>

<div class="project-block">
  <div class="project-text">

<p style="color: #2f6db5; font-weight: 700; font-size: 1.2rem; margin-bottom: 0.5rem;">
Epidemiological Focus:
</p>
My work develops practical approaches for handling 
incomplete and censored data in epidemiologic studies.

  </div>
</div>

**Selected publications:**

- Gillespie, B. W., **Chen, Q.**, Reichert, H., Franzblau, A., Lepkowski, J., Adriaens, P., Demond, A., Luksemburg, W., and Garabrant, D. (2010). “Estimating population distributions when some data are below a limit of detection by using a reverse Kaplan-Meier estimator”, *Epidemiology*, **21**, S64–S70.

- **Chen, Q.**, Williams, S. Z., Liu, Y., Chihuri, S. T., and Li, G. (2018). “Multiple imputation of missing marijuana data in the Fatality Analysis Reporting System using a Bayesian multilevel model”, *Accident Analysis and Prevention*, **120**, 262–269.

<div style="height: 40px;"></div>

<div class="bottom-nav">
  <a class="bottom-nav-btn" href="/lab/project/measurement_error/" aria-label="Previous">
    ← Previous
  </a>
  <a class="bottom-nav-btn" href="/lab/project/epi_research/" aria-label="Next">
    Next →
  </a>
</div>

