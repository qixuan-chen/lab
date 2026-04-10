# 

<style>
/* --- Tabs (no JS) --- */
.tabs2 {
  max-width: 900px;
  margin: 0 auto;
}
.tabs2 input[type="radio"] { display: none; }
.tabs2 .tab-labels{
  display:flex; gap:10px;
  border-bottom:1px solid rgba(0,0,0,.12);
  margin-bottom:18px;
}
.tabs2 .tab-labels label{
  cursor:pointer;
  padding:10px 14px;
  border-radius:10px 10px 0 0;
  font-weight:600;
  opacity:.7;
  user-select:none;
}
.tabs2 .tab-content{ display:none; padding:6px 0 0 0; }

/* active state */
#tab-dash:checked ~ .tab-labels label[for="tab-dash"],
#tab-rpkg:checked ~ .tab-labels label[for="tab-rpkg"]{
  opacity:1;
  border-bottom:3px solid currentColor;
}
#tab-dash:checked ~ .content #content-dash,
#tab-rpkg:checked ~ .content #content-rpkg{ display:block; }


.tabs2 .project-row{
  display:flex;
  align-items:flex-start;
  gap:18px;
  margin: 6px 0 22px;
}
.tabs2 .project-text{ flex: 1 1 auto; min-width: 240px; }
.tabs2 .project-text h3{ margin: 0 0 8px; }
.tabs2 .project-text p{ margin: 0 0 10px; }

.tabs2 .project-media{
  flex: 0 0 320px;         
  max-width: 40%;
}
.tabs2 .project-media img{
  width: 100%;
  height: 200px;         
  object-fit: cover;     
  border-radius: 12px;
  display: block;
}

.tight-title{
  margin-bottom: 4px;
}

.tight-text{
  margin-top: 0;
  margin-bottom: 10px;
}

.desc-text{
  color: #8a8a8a;
}

.pkg-divider{
  height: 1px;
  background: #e5e7eb;
  margin: 18px 0;
}

.press-date-line{
  text-align: right;
  font-size: 0.9rem;
  opacity: 0.75;
  margin-top: 0.25rem;   
  margin-bottom: -0.25rem; 
}

.pkg-item {
  margin-bottom: 0;
}

#pkgSort {
  padding: 4px 8px;
  border-radius: 6px;
}

@media (max-width: 760px){
  .tabs2 .project-row{ flex-direction:column; }
  .tabs2 .project-media{ flex-basis:auto; max-width:100%; }
}
</style>

<div class="tabs2">
  <input id="tab-dash" type="radio" name="tabs2" checked>
  <input id="tab-rpkg" type="radio" name="tabs2">

  <div class="tab-labels">
    <label for="tab-dash">Dashboards</label>
    <label for="tab-rpkg">R packages</label>
  </div>

  <div class="content">
    <div id="content-dash" class="tab-content">
      <div class="project-row">
        <div class="project-text">
          <h3>COVID-19 Dashboard</h3>
          <p>Real-time tracking and analysis of COVID-19 trends in New York City.</p>
          <p><a href="https://msph.shinyapps.io/nyc-neighborhoods-covid/" target="_blank" rel="noopener">Read more</a></p>
        </div>
        <div class="project-media">
          <img src="/images/press/ncd-1500x632.jpg" alt="COVID Dashboard" />
        </div>
      </div>
      <div class="project-row">
        <div class="project-text">
          <h3>Lung Disease Diagnostic Tool</h3>
          <p>This Shiny app is designed for implementing the radiology diagnostic tool</p>
          <p><a href="https://msph.shinyapps.io/DiagnosticApp/" target="_blank" rel="noopener">Read more</a></p>
        </div>
        <div class="project-media">
          <img src="/images/press/prime_logo.png" alt="Lung disease Dashboard" />
        </div>
      </div>
      <div class="project-row">
        <div class="project-text">
          <h3>Survey Weighting App</h3>
          <p>This tool is designed to facilitate high-quality survey data analysis and improve the accuracy and reliability of estimates through appropriate weighting techniques.</p>
          <p><a href=" https://kindle0118.shinyapps.io/weighting/" target="_blank" rel="noopener">Read more</a></p>
        </div>
        <div class="project-media">
          <img src="/images/press/background.png" alt="Lung disease Dashboard" />
        </div>
      </div>
    </div>
    <div id="content-rpkg" class="tab-content">
      <div style="text-align:right; margin-bottom:12px;">
        Sort by:
        <select id="pkgSort">
          <option value="desc">reverse</option>
          <option value="asc">chronological</option>
        </select>
      </div>
      <div id="pkgList">
        <div class="pkg-item" data-year="2013">
          <h3 class="tight-title">MI-lasso for multiply-imputed data</h3>
          <p class="tight-text">
            Available as the <a href="https://www.columbia.edu/~qc2138/Downloads/software/MI_lasso%20macro.sas" target="_blank" rel="noopener">%MI_lasso</a> SAS macro and
            <a href="https://www.columbia.edu/~qc2138/Downloads/software/MI-lasso.R" target="_blank" rel="noopener">MI.lasso</a> R function.
          </p>
          <p class="tight-text desc-text">
            An implementation of the MI-lasso variable selection method that extends
            the lasso method to multiply-imputed data. The MI-lasso treats the 
            regression coefficients of the same covariate across all imputed datasets 
            as a group and applies the group lasso penalty to yield a consistent 
            variable selection across all imputed datasets.
          </p>
          <h4 class="tight-title">Reference:</h4>
          <p class="tight-text">
            Chen, Q. and Wang, S. (2013). Variable selection for multiply-imputed 
            data with application to dioxin exposure study, <em>Statistics in Medicine</em>, 
            <strong>32</strong>, 3646–59. 
            <a href="https://www.columbia.edu/~qc2138/Downloads/Chen_SIM2013/Chen_2013_SIM.pdf" target="_blank" rel="noopener">[PDF]</a>
          </p>
          <div class="press-date-line">2013</div>
          <div class="pkg-divider"></div>
        </div>
        <div class="pkg-item" data-year="2016">
          <h3 class="tight-title">Logistic partially linear models with missing covariates</h3>
          <p class="tight-text">
            Available in <a href="https://www.columbia.edu/~qc2138/Downloads/software/CSDA2016/R_CSDA2016.pdf" target="_blank" rel="noopener">this supplement</a>.
          </p>
          <p class="tight-text desc-text">
            We propose a new kernel-assisted estimating equation method for logistic
            partially linear models with missing covariates.
          </p>
          <h4 class="tight-title">Reference:</h4>
          <p class="tight-text">
            Chen, Q., Paik, M. C., Kim, M., and Wang, C. (2016). Using link-preserving
            imputation for logistic partially linear models with missing covariates,
            <em>Computational Statistics and Data Analysis</em>, <strong>101</strong>, 174–185.
            <a href="https://www.sciencedirect.com/science/article/pii/S0167947316300411" target="_blank" rel="noopener">[Link]</a>
          </p>
          <div class="press-date-line">2016</div>
          <div class="pkg-divider"></div>
        </div>
        <div class="pkg-item" data-year="2023">
          <h3 class="tight-title">Bivariate hierarchical Bayesian model for combining summary measures</h3>
          <p class="tight-text">
            Available in <a href="https://github.com/yaoyuanj/BHSM" target="_blank" rel="noopener">this github repository</a>.
          </p>
          <p class="tight-text desc-text">
            This package implements a bivariate hierarchical Bayesian model for
            combining summary measures and their uncertainties from multiple sources.
            It is suitable for applications such as meta-analysis, PET brain imaging,
            and small area estimation.
          </p>
          <h4 class="tight-title">Reference:</h4>
          <p class="tight-text">
            Yao, Y., Ogden, R. T., Zeng, C., and Chen, Q. (2023). Bivariate 
            hierarchical Bayesian model for combining summary measures and their 
            uncertainties from multiple sources, <em>The Annals of Applied Statistics</em>,
            <strong>17</strong>(2), 1782–1800. 
            <a href="https://doi.org/10.1214/22-AOAS1699" target="_blank" rel="noopener">[DOI]</a>
          </p>
          <div class="press-date-line">2023</div>
          <div class="pkg-divider"></div>
        </div>
        <div class="pkg-item" data-year="2024">
          <h3 class="tight-title">Auxiliary-data-assisted Survey Inference Using Administrative Records</h3>
          <p class="tight-text">
            Available as <strong>AuxSurvey</strong> R package in 
            <a href="https://github.com/zjg540066169/AuxSurvey" target="_blank" rel="noopener">this github repository</a>.
          </p>
          <p class="tight-text desc-text">
            AuxSurvey is an R package for auxiliary-data-assisted survey inference 
            using administrative records when individual-level continuous auxiliary
            variables cannot be publicly released. It implements a two-step Bayesian 
            predictive inference strategy that combines discretized auxiliary variables 
            with estimated inclusion propensities, and supports the GAMP 
            (generalized additive model of propensity) approach to improve efficiency 
            and coverage in survey estimation.
          </p>
          <h4 class="tight-title">Reference:</h4>
          <p class="tight-text">
            Williams, S. Z., Zou, J., Liu, Y., Si, Y., Galea, S., and Chen, Q. (2024). 
            Improving survey inference using administrative records without releasing 
            individual-level continuous data, <em>Statistics in Medicine</em>, <strong>43</strong>, 5803–5813. 
            <a href="https://doi.org/10.1002/sim.10270" target="_blank" rel="noopener">[DOI]</a>
          </p>
          <div class="press-date-line">2024</div>
          <div class="pkg-divider"></div>
        </div>
        <div class="pkg-item" data-year="2025">
          <h3 class="tight-title">BMIselect: Bayesian MI-LASSO for Variable Selection on Multiply-Imputed Datasets</h3>
          <p class="tight-text">
            Available as <strong>BMIselect</strong> R package in 
            <a href="https://cran.r-project.org/web/packages/BMIselect/index.html" target="_blank" rel="noopener">this CRAN repository</a>.
          </p>
          <p class="tight-text desc-text">
            Provides a suite of Bayesian MI-LASSO for variable selection methods 
            for multiply-imputed datasets. The package includes four Bayesian MI-LASSO 
            models using shrinkage (Multi-Laplace, Horseshoe, ARD) and Spike-and-Slab 
            (Spike-and-Laplace) priors, along with tools for model fitting via MCMC, 
            four-step projection predictive variable selection, and hyperparameter calibration. 
            Methods are suitable for both continuous and binary covariates under missing-at-random 
            or missing-completely-at-random assumptions. We also provide the frequentist's MI-LASSO function.
          </p>
          <h4 class="tight-title">Reference:</h4>
          <p class="tight-text">
            Zou, J., Wang, S., and Chen, Q. (2025). Bayesian MI-LASSO for Variable Selection 
            on Multiply-Imputed Data, <em>arXiv</em>, arXiv:2211.00114. 
            <a href="https://doi.org/10.48550/arXiv.2211.00114" target="_blank" rel="noopener">[DOI]</a>
          </p>
          <div class="press-date-line">2025</div>
          <div class="pkg-divider"></div>
        </div>
      </div>
    </div>
    
<script>
document.addEventListener("DOMContentLoaded", function() {
  const sortSelect = document.getElementById("pkgSort");
  const pkgList = document.getElementById("pkgList");
  if (!sortSelect || !pkgList) return;

  function renderPkgList(order) {
    const items = Array.from(pkgList.querySelectorAll(".pkg-item"));

    items.sort((a, b) => {
      const yearA = parseInt(a.dataset.year);
      const yearB = parseInt(b.dataset.year);
      return order === "asc" ? yearA - yearB : yearB - yearA;
    });

    pkgList.innerHTML = "";
    items.forEach(item => pkgList.appendChild(item));
  }

  renderPkgList("desc");

  sortSelect.addEventListener("change", function() {
    renderPkgList(this.value);
  });
});
</script>
