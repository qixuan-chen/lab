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
  <div class="page-banner" style="background-image:url('/images/research/survey.png');"></div>

  <div class="page-nav">
    <a class="nav-btn nav-back" href="/research/" aria-label="Back to Research">
      ← Back
    </a>
  </div>
</div>

<div class="banner-title">Bayesian Survey Inference</div>

My research develops Bayesian methods for population-level inference from both 
probability and nonprobability data, integrating flexible modeling with external
data sources to address complex survey features and enhance generalizability.

<div style="height: 20px;"></div>

<div class="project-block">
  <div class="project-text">
§ denote trainees.

<p style="color: #2f6db5; font-weight: 700; font-size: 1.2rem; margin-bottom: 0.5rem;">
  Bayesian Predictive Inference from Nonprobability Samples:
</p> 
My recent work focuses on predictive inference from nonprobability samples using Bayesian machine 
learning methods. This research integrates nonprobability samples with external 
data sources—including administrative records, electronic health records, 
aggregated population data, and probability surveys—to make population-level 
inference. The goal is to develop approaches that enhance the generalizability 
of inferences drawn from nonprobability data.

  </div>
</div>

**Selected publications:**
- Liu, Y.§, Gelman, A., **Chen, Q.** (2023). “Inference from non-random samples using Bayesian machine learning”, *Journal of Survey Statistics and Methodology*, **11**(2), 433–455.

- Williams, S.§, Zou, J., Liu, Y., Si, Y., Galea, S., and **Chen, Q.** (2024). “Improving survey inference using administrative records without releasing individual-level continuous data”, *Statistics in Medicine*, **43**, 5803–5813.

- Pitts, A.§, Yomogida, M., Aidala, A., Gelman, A., and **Chen, Q.** (2025). “Multilevel Regression and Poststratification using Margins of Post-Stratifiers: Improving Inference for HIV Health Outcomes During the COVID-19 Pandemic”, *Statistics in Medicine*, **44**(18–19), e70223.

- Wang, X.§, Zhu, A.§, Kennedy, L., Greenleaf, A., and **Chen, Q.** (2026). “Improving survey inference in nested-cohort samples using Bayesian machine learning”, *Journal of the Royal Statistical Society: Series A*. DOI: [10.1093/jrsssa/qnaf136](https://doi.org/10.1093/jrsssa/qnaf136).

<div style="height: 20px;"></div>

<div class="project-block">
  <div class="project-text">

<p style="color: #2f6db5; font-weight: 700; font-size: 1.2rem; margin-bottom: 0.5rem;">
Bayesian Model-Based Survey Inference:
</p>
My work on inference of population 
quantities from probability surveys leverages flexible Bayesian models. This 
approach incorporates key design variables directly into Bayesian modeling, 
enabling the handling of complex survey features such as clustering, 
stratification, unequal probabilities of selection, and informative sampling.

  </div>
</div>

**Selected publications:**
- **Chen, Q.**, Elliott, M. R., and Little, R. J. A. (2010). “Bayesian penalized spline model-based inference for finite population proportion in unequal probability sampling”, *Survey Methodology*, **36**, 23–34.

- **Chen, Q.**, Elliott, M. R., and Little, R. J. A. (2012). “Bayesian inference of finite population quantiles from unequal probability samples”, *Survey Methodology*, **38**, 203–214.

- **Chen, Q.**, Elliott, M., Haziza, D., Yang, Y., Ghosh, M., Little, R. J. A., Sedransk, J., and Thompson, M. (2017). “Approaches to improving survey-weighted estimates”, *Statistical Science*, **32**(2), 227–248.

- Liu, Y.§, **Chen, Q.** (2020). “Bayesian Inference of Finite Population Quantiles for Skewed Survey Data Using Skew-Normal Penalized Spline Regression”, *Journal of Survey Statistics and Methodology*, **8**(4), 792–816.

- Sedransk, J., Tang, H.§, and **Chen, Q.** “Bayesian analytic inference under informative sampling”, submitted.

<div style="height: 20px;"></div>

<div class="project-block">
  <div class="project-text">

<p style="color: #2f6db5; font-weight: 700; font-size: 1.2rem; margin-bottom: 0.5rem;">
Bayesian Modeling of Survey Data:
</p>
My work develops Bayesian methods for 
analyzing complex survey data, addressing challenges such as multilevel structure, 
latent heterogeneity, data integration, and model validation. These studies 
provide practical modeling strategies and highlight potential pitfalls, advancing
reliable inference for population-level analyses.

  </div>
</div>

**Selected publications:**

- Thompson, M., Meng, G., Sedransk, J., **Chen, Q.**, Anthopolos, R., and Galea, S. (2022). “Spatial Multilevel Modelling in the Galveston Bay Recovery Study Survey.” In *Advances and Innovations in Statistics and Data Science* (pp. 275–293), Springer.

- Anthopolos, R.§, **Chen, Q.**, Sedransk, J., Thompson, M., Meng, G., and Galea, S. (2023). “A Bayesian growth mixture model for complex survey data: clustering post-disaster PTSD trajectories”, *Annals of Applied Statistics*, **17**(3), 2494–2514.

- Yao, Y.§, Ogden, T., Zeng, C., and **Chen, Q.** (2023). “Bivariate hierarchical Bayesian model for combining summary measures and their uncertainties from multiple sources”, *Annals of Applied Statistics*, **17**(2), 1782–1800.

- Kuh, S., Kennedy, L., **Chen, Q.**, and Gelman, A. (2024). “Using leave-one-out cross validation (LOO) in a multilevel regression and poststratification (MRP) workflow: A cautionary tale”, *Statistics in Medicine*, **43**(5), 953–982.

- Kuh, S., Kennedy, L., **Chen, Q.**, and Gelman, A. “When Bayes goes bad: Weakly-regularized covariate adjustment leads to a biased estimate of prevalence”, submitted.

<div style="height: 40px;"></div>

<div class="bottom-nav">
  <a class="bottom-nav-btn" href="/research/" aria-label="Previous">
    ← Previous
  </a>
  <a class="bottom-nav-btn" href="/project/health_app/" aria-label="Next">
    Next →
  </a>
</div>
