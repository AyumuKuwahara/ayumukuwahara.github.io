---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}


## Primary interest: disk-planet interaction


<style>
.grid-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 20px;
  margin-top: 20px;
}
.grid-item {
  text-align: center;
}
.grid-item img {
  width: 100%;
  height: 300px; /* ★ここで高さを統一 */
  object-fit: cover; /* ★画像を切り取りながら枠にフィット */
  border-radius: 8px;
}
</style>

<div class="grid-container">
  <div class="grid-item">
    <img src="/images/envelope.jpg" alt="Project 1">
    <p><strong>Gas flow around embedded planets</strong><br>Planets embedded in protoplanetary disks perturb the surrounding gas. I simulate the resulting gas dynamics using the public hydrodynamics code Athena++.</p>
  </div>
  <div class="grid-item">
    <img src="/images/3D_trajectories.gif" alt="Project 2">
    <p><strong>Pebble accretion</strong><br>Planets accrete millimeter- to centimeter-sized particles, known as pebbles. These pebbles are strongly coupled to the gas flow. I simulate pebble dynamics by post-processing hydrodynamical simulation data.</p>
  </div>
    <div class="grid-item">
    <img src="/images/output.gif" alt="Project 3">
    <p><strong>Gas accretion onto gap-opening planets</strong><br>Giant planets undergo runaway gas accretion in the disk. I simulate the disk–planet interaction and the gas accretion process using the public hydrodynamics code Athena++.</p>
  </div>
  <div class="grid-item">
    <img src="/images/141105_ALMA_HL_01.jpg" alt="Project 4">
    <p><strong>Dust ring and gap formation by low-mass planets</strong><br>Observed dust rings and gaps in protoplanetary disks may be signatures of forming planets. We show that an Earth-mass planet at 10 au can generate prominent dust rings and gaps. Image Credit: ALMA (/NRAO/ESO/NAOJ)</p>
  </div>
</div>