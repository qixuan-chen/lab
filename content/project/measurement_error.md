---
title: ""
draft: false
---

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
  <div class="page-banner" style="background-image:url('/lab/images/research/measurement.jpg');"></div>

  <div class="page-nav">
    <a class="nav-btn nav-back" href="/lab/research/" aria-label="Back to Research">
      ← Back
    </a>
  </div>
</div>

<div class="banner-title">Measurement Error</div>

My research develops statistical and epidemiologic methods to address measurement
error and misclassification in complex data settings. 

<div style="height: 20px;"></div>

<div class="project-block">
  <div class="project-text">
§ denote trainees.

<p style="color: #2f6db5; font-weight: 700; font-size: 1.2rem; margin-bottom: 0.5rem;">
Statistical Focus:
</p>
I develop robust statistical methods to correct for
measurement error in environmental epidemiology and biomedical assays. I have
introduced novel methods to handle complex data challenges such as multiple 
correlated exposures, mixed continuous and discrete covariates, and sample 
contamination. 

  </div>
</div>

**Selected publications:**

- Yu, Y.§, Little, R. J. A., Perzanowski, M., and **Chen, Q.** (2024). “Multiple imputation of more than one environmental exposure with non-differential measurement error”, *Biostatistics*, **25**(2), 306–322.

- Wang, S.§, **Chen, Q.**, Perzanowski, M., Divjan, A., and Gelman, A. “A Bayesian contamination model for serial dilution assays”, *Biometrics*, revision submitted.

- Kwizera, M. H.§, **Chen, Q.**, Perzanowski, M., and Little, R. J. “A general location model approach to measurement error adjustment in regression settings with mixed continuous and discrete variables”, submitted.

<div style="height: 20px;"></div>

<div class="project-block">
  <div class="project-text">

<p style="color: #2f6db5; font-weight: 700; font-size: 1.2rem; margin-bottom: 0.5rem;">
Epidemiological Focus:
</p>
My work focuses on understanding and correcting for 
measurement error and misclassification in epidemiologic studies. 

  </div>
</div>

**Selected publications:**

- **Chen, Q.**, Galfalvy, H., and Duan, N. (2013). “Effects of disease misclassification on exposure-disease association”, *American Journal of Public Health*, **103**, e67–e73.

- Jin, H.§, Williams, S., Chihuri, S., Li, G., and **Chen, Q.** (2018). “Validity of oral fluid test for Delta-9-Tetrahydrocannabinol in drivers using the 2013 National Roadside Survey Data”, *Injury Epidemiology*, **5**, 3.

- Lee, S.§, Li, G., Chihuri, S. T., Yu, Y.§, and **Chen, Q.** (2024). “Using data fusion with multiple imputation to correct for misclassification in self-reported exposure: a case-control study of cannabis use and homicide victimization”, *Injury Epidemiology*, **11**, 57.

<div style="height: 40px;"></div>

<div class="bottom-nav">
  <a class="bottom-nav-btn" href="/lab/project/health_app/" aria-label="Previous">
    ← Previous
  </a>
  <a class="bottom-nav-btn" href="/lab/project/missing_data/" aria-label="Next">
    Next →
  </a>
</div>
