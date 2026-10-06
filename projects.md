---
layout: default
---

<div class="projects-wide">
<h3>Projects</h3>
<div class="project-grid">
  <div class="project-card">
    <img src="images/inverse_algorithm.jpg" alt="Novel sequential inversion algorithm">
    <div class="project-body">
      <div class="project-title">Novel Sequential Inversion Algorithm</div>
      <p>Our sequential inversion algorithm uses a borewell-scale, physics-based model to estimate aquifer parameters.</p>
      <p><a href="https://doi.org/10.1016/j.jhydrol.2026.135967" target="_blank">Read the paper</a></p>
    </div>
  </div>
  <div class="project-card">
    <img src="images/sy.jpg" alt="Billions of inverse simulations to estimate subsurface parameters at continental scale">
    <div class="project-body">
      <div class="project-title">Continental-scale Parameter Estimation</div>
      <p>Billions of inverse simulations on a parallel computing architecture, run on the <a href="https://www.serc.iisc.ac.in/supercomputer/for-traditional-hpc-simulations-param-pravega/" target="_blank">PARAM Pravega</a> supercomputer, using our <a        href="https://doi.org/10.1016/j.jhydrol.2026.135967" target="_blank">sequential inversion algorithm</a>.</p>
    </div>
  </div>
  <div class="project-card">
    <img src="images/lake_recharge.jpg" alt="Modelling subsurface recharge through Lakes">
    <div class="project-body">
      <div class="project-title">Lake Recharge Modelling</div>
      <p>MODFLOW models quantifying artificial recharge through lakes.</p>
      <p><a href="#" target="_blank">link</a></p>
    </div>
  </div>
  <div class="project-card">
    <img src="images/bial_modflow.jpg" alt="Numerical simulation of groundwater flow">
    <div class="project-body">
      <div class="project-title">Numerical Simulation of Groundwater Flow</div>
      <p>Numerical simulations to estimate groundwater resources at Bengaluru International Airport (BIAL).</p>
    </div>
  </div>
  <div class="project-card">
    <img src="images/ml_flow.jpg" alt="Surrogate and hybrid numerical models">
    <div class="project-body">
      <div class="project-title">Surrogate / Hybrid Physics-ML Models</div>
      <p>Training ML models on numerical model simulations to build fast surrogates for quick predictions.</p>
    </div>
  </div>
</div>
</div>

<script>
document.addEventListener('DOMContentLoaded', function () {
  var box = document.createElement('div');
  box.className = 'lightbox';
  var big = document.createElement('img');
  box.appendChild(big);
  document.body.appendChild(box);
  document.querySelectorAll('.project-card img').forEach(function (img) {
    img.addEventListener('click', function () {
      big.src = img.src;
      big.alt = img.alt;
      box.classList.add('open');
    });
  });
  box.addEventListener('click', function () { box.classList.remove('open'); });
  document.addEventListener('keydown', function (e) {
    if (e.key === 'Escape') { box.classList.remove('open'); }
  });
});
</script>
