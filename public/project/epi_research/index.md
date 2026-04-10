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
  <div class="page-banner" style="background-image:url('/lab/images/research/epidemiological.jpg');"></div>

  <div class="page-nav">
    <a class="nav-btn nav-back" href="/lab/research/" aria-label="Back to Research">
      ← Back
    </a>
  </div>
</div>

<div class="banner-title">Epidemiologic Research</div>

Alongside the developments of new statistical methods, I lead applied research 
in epidemiology and biomedical science, publishing as a first or senior author 
in epidemiologic and medical journals. My research integrates advanced statistical 
and machine learning methods across environmental health, COVID-19 studies, 
and radiology diagnostics to address key public health and clinical questions.

<div style="height: 20px;"></div>

<div class="project-block">
  <div class="project-text">
§ denote trainees.

<p style="color: #2f6db5; font-weight: 700; font-size: 1.2rem; margin-bottom: 0.5rem;">
Environmental Health Sciences:
</p>
I applied advanced statistical methods to 
environmental health studies, including quantile regression and latent class 
growth analysis, to characterize environmental exposures and identify disease 
phenotypes and trajectories in population-based cohorts.

  </div>
</div>

**Selected publications:**

- **Chen, Q.**, Garabrant, D., Hedgeman, E., Little, R. J. A., Elliott, M. R., Gillespie, B., Hong, B., Lee, S., Lepkowski, J., Franzblau, A., Adriaens, P., Demond, A., and Patterson, D. (2010). “Estimation of background serum 2,3,7,8-TCDD concentrations by using quantile regression in the UMDES and NHANES populations”, *Epidemiology*, **21**, S51–S57.

- **Chen, Q.**, Just, A. C., Miller, R. L., Perzanowski, M. S., Goldstein, I. F., Perera, F. P., and Whyatt, R. M. (2012). “Using latent class growth analysis to identify childhood wheeze phenotypes in an urban birth cohort”, *Annals of Allergy, Asthma & Immunology*, **108**, 311–315.e1.

- **Chen, Q.**, Jiang, X., Garabrant, D., Hedgeman, E., Gillespie, B., Hong, B., Lepkowski, J., Franzblau, A., and Jolliet, O. (2013). “Estimation of age- and sex-specific background human serum concentrations of PCDDs, PCDFs, and PCBs in the UMDES and NHANES populations”, *Chemosphere*, **91**, 817–823.

- **Chen, Q.**, Zhong, X., Acosta, L., Divjan, A., Rundle, A., Goldstein, I. F., Miller, R. L., and Perzanowski, M. S. (2016). “Allergic sensitization patterns identified through Latent Class Analysis among NYC asthmatic and non-asthmatic children”, *Annals of Allergy, Asthma and Immunology*, **116**(3), 212–218.

- Flores, N. M.§, Perzanowski, M. S., Lovinsky-Desir, S., Divjan, A., Hoepner, L. A., Miller, R. L., Herbstman, J. B., Perera, F. P., and **Chen, Q.** (2024). “Trajectory analysis of rhinitis in a birth cohort from lower-income NYC neighborhoods”, *Journal of Allergy and Clinical Immunology*, **154**(1), 111–119. *(Note: This paper was selected for JACI Editorial.)*

<div style="height: 20px;"></div>

<div class="project-block">
  <div class="project-text">

<p style="color: #2f6db5; font-weight: 700; font-size: 1.2rem; margin-bottom: 0.5rem;">
COVID-19 Studies:
</p>
My lab developed a NYC Neighborhood COVID-19 dashboard to 
track and visualize real-time data and conducted epidemiologic research on 
neighborhood-level disparities in health outcomes and their broader impacts.
I also led the design and analysis of a cellphone survey in Lesotho to monitor 
trajectories of flu-like symptoms between 2020 and 2021.

  </div>
</div>

**Selected publications:**

- Zhong, X., Zhou, Z.§, Li, G., Muhire, Z., Muennig, P., and **Chen, Q.** (2022). “Neighborhood disparities in COVID-19 outcomes in New York City over the two waves of the outbreak”, *Annals of Epidemiology*, **70**, 45–52.

- Olawole, W.§, Li, G., Zhou, Z.§, Wu, Z.§, and **Chen, Q.** (2024). “Association between neighborhood-level COVID-19 mortality and the increase in drug overdose mortality in New York City during the COVID-19 pandemic”, *Injury Epidemiology*, **11**, 65.

- Greenleaf, A. R.§, Francis, S., Zou, J., Farley, S. M., Lekhela, T., Asiimwe, F., and **Chen, Q.** (2024). “Influenza-like illness symptoms as reported by a population-based participatory surveillance system in Lesotho, July 2020–July 2021”, *JMIR Public Health and Surveillance*, **10**, e55208.

<div style="height: 20px;"></div>

<div class="project-block">
  <div class="project-text">

<p style="color: #2f6db5; font-weight: 700; font-size: 1.2rem; margin-bottom: 0.5rem;">
Radiology Diagnosis:
</p>
My lab developed a machine learning–based radiology 
model for pulmonary fibrosis and implemented it as a Shiny app.

  </div>
</div>

**Selected publications:**

- Fan, W.§, **Chen, Q.**, Maccarrone, V., Luk, L., Navot, B., and Salvatore, M. (2024). “Developing radiology diagnosis tools for pulmonary fibrosis using machine learning methods”, *Clinical Imaging*, **106**, 110047.

- Fan, W.§, **Chen, Q.**, Luk, L., Navot, B., Maccarrone, V., and Salvatore, M. (2024). “Use of a radiology tool for the diagnosis of pulmonary fibrosis”, *Clinical Imaging*, **115**, 110277.

<div style="height: 40px;"></div>

<div class="bottom-nav">
  <a class="bottom-nav-btn" href="/lab/project/missing_data/" aria-label="Previous">
    ← Previous
  </a>
  <a class="bottom-nav-btn" href="/lab/research/" aria-label="Next">
    Next →
  </a>
</div>

