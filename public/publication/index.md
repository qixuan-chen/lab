# 



<style>
.sym-btn{
  margin-left: 8px;
  padding: 6px 10px;
  border: 1px solid rgba(0,0,0,.18);
  border-radius: 10px;
  background: transparent;
  cursor: pointer;
  font-size: 14px;
}
.sym-btn[aria-pressed="true"]{
  border-color: rgba(0,0,0,.35);
  box-shadow: 0 6px 16px rgba(0,0,0,.10);
}

/* 符号默认不变色 */
.sym{
  color: inherit;
  font-weight: inherit;
}

.highlight-star  .sym-star{ color:#c62828; font-weight:700; }
.highlight-section .sym-section{ color:#1565c0; font-weight:700; }
.highlight-corresp .sym-corresp{ color:#2e7d32; font-weight:700; }

.year-header{
  font-size: 22px;
  font-weight: 700;
  margin-top: 36px;
  margin-bottom: 10px;
  border-bottom: 2px solid rgba(0,0,0,.12);
  padding-bottom: 4px;
}

.pub-item{
  display: grid;
  grid-template-columns: 44px minmax(0, 1fr);
  column-gap: 10px;
  margin-bottom: 18px;
  align-items: start;
}

.pub-no{
  font-weight: 700;
  opacity: 0.75;
}


.pub-item > :not(.pub-no){
  min-width: 0;
  white-space: normal;
  overflow-wrap: anywhere;  
  word-break: normal;
}

</style>

<br>

Visit my [Google Scholar profile](http://scholar.google.com/citations?user=gHLwOp4AAAAJ&hl=en&oi=ao).

<br>

### Peer-Reviewed Research Publications

<p style="margin-top:8px;">
  <span class="legend-text">
    <code>*</code> is used to indicate first or senior authorship; 
    <code>§</code> is used to indicate student or mentee; 
    <code>&#9993</code> is used to indicate corresponding author.
  </span>


</p>
<div style="clear:both;"></div>


<div style="text-align:right; margin-bottom:10px;">
Sort by:
<select id="pubSort">
  <option value="desc">reverse</option>
  <option value="asc">chronological</option>
</select>
</div>

<div id="pubList">

<div class="pub-item" data-year="2026">
  <span class="pub-no">1.</span>
  <div class="pub-body">
    * Wang, X.<sup>§</sup>, Zhu, A.<sup>§</sup>, Kennedy, L., Greenleaf, A., and 
    <strong>Chen, Q.<sup>&#9993;</sup></strong> (2026).
    <em>"Improving survey inference in nested-cohort samples using Bayesian machine learning."</em>
    <em>Journal of the Royal Statistical Society: Series A.</em>
    <a href="https://doi.org/10.1093/jrsssa/qnaf136">DOI: 10.1093/jrsssa/qnaf136</a>
  </div>
</div>


<div class="pub-item" data-year="2025">
<span class="pub-no"></span>
<strong>Pitts, A.§, Yomogida, M., Aidala, A., Gelman, A., and Chen, Q. (2025).</strong><br>
<em>Multilevel Regression and Poststratification using Margins of Post-Stratifiers.</em><br>
<em>Statistics in Medicine, 44(18–19): e70223.</em>
</div>

<div class="pub-item" data-year="2025">
<span class="pub-no"></span>
<strong>Farley, S.M., Delgado, S., ... El-Sadr, W.M. (2025).</strong><br>
<em>Assessment of a gridded population sample frame...</em><br>
<em>International Journal of Health Geographics, 24(1): 47.</em>
</div>

<div class="pub-item" data-year="2025">
<span class="pub-no"></span>
<strong>Fnu, T., Shi, P., ... Que, J. (2025).</strong><br>
<em>The SOX4-Semaphorin3C axis promotes Esophageal Adenocarcinoma progression.</em><br>
<em>Cancer Letters, 633: 218005.</em><br>
<em>DOI: 10.1016/j.canlet.2025.218005.</em><br>
</div>

</div>


<script>
document.addEventListener("DOMContentLoaded", function() {
  const sortSelect = document.getElementById("pubSort");
  const pubList = document.getElementById("pubList");

  function renderList(order) {
    const items = Array.from(pubList.querySelectorAll(".pub-item"));

  
    items.sort((a, b) => {
      const yearA = parseInt(a.dataset.year);
      const yearB = parseInt(b.dataset.year);
      return order === "asc" ? yearA - yearB : yearB - yearA;
    });

  
    pubList.innerHTML = "";

    let currentYear = null;
    let idx = 1;

    items.forEach(item => {
      const year = item.dataset.year;


      if (year !== currentYear) {
        currentYear = year;
        const header = document.createElement("div");
        header.className = "year-header";
        header.textContent = year;
        pubList.appendChild(header);
      }

     
      const no = item.querySelector(".pub-no");
      if (no) no.textContent = idx + ".";
      idx++;

      pubList.appendChild(item);
    });
  }


  renderList("desc");

  sortSelect.addEventListener("change", function() {
    renderList(this.value);
  });
});
</script>



<script>
document.addEventListener("DOMContentLoaded", () => {
  const pubList = document.getElementById("pubList");
  if (!pubList) return;

  
  const wrapSymbolsInTextNode = (textNode) => {
    const text = textNode.nodeValue;
    if (!text || !/[\*\§\%]/.test(text)) return;

    const frag = document.createDocumentFragment();
    const parts = text.split(/([\*\§\%])/); 

    parts.forEach(part => {
      if (part === "*") {
        const s = document.createElement("span");
        s.className = "sym sym-star";
        s.textContent = "*";
        frag.appendChild(s);
      } else if (part === "§") {
        const s = document.createElement("span");
        s.className = "sym sym-section";
        s.textContent = "§";
        frag.appendChild(s);
      } else if (part === "%") {
        const s = document.createElement("span");
        s.className = "sym sym-corresp";
        s.textContent = "%";
        frag.appendChild(s);
      } else if (part.length) {
        frag.appendChild(document.createTextNode(part));
      }
    });

    textNode.parentNode.replaceChild(frag, textNode);
  };


  const walker = document.createTreeWalker(pubList, NodeFilter.SHOW_TEXT, {
    acceptNode(node) {
      const p = node.parentNode && node.parentNode.nodeName;
      if (p === "SCRIPT" || p === "STYLE") return NodeFilter.FILTER_REJECT;
      if (!/[\*\§\%]/.test(node.nodeValue || "")) return NodeFilter.FILTER_SKIP;
      return NodeFilter.FILTER_ACCEPT;
    }
  });

  const toWrap = [];
  while (walker.nextNode()) toWrap.push(walker.currentNode);
  toWrap.forEach(wrapSymbolsInTextNode);


  const toggleMap = {
    star: "highlight-star",
    section: "highlight-section",
    corresp: "highlight-corresp"
  };

  document.querySelectorAll(".sym-btn[data-toggle]").forEach(btn => {
    btn.addEventListener("click", () => {
      const key = btn.getAttribute("data-toggle");
      const cls = toggleMap[key];
      const isOn = document.body.classList.toggle(cls);
      btn.setAttribute("aria-pressed", String(isOn));
    });
  });
});
</script>
