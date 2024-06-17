## CFD: Simulating flow around a wing

![](images/intro/drawing-cfd.png)

vvv

## FEM: Simulating stresses on a wing

![](images/intro/drawing-fem.png)

vvv

## Can we simulate both at the same time?

![](images/intro/drawing-fsi-monolithic.png)

vvv

## ...but reusing the CFD and FEM codes?

![](images/intro/drawing-fsi-partitioned.png)

vvv

## From the CFD world to the FEM world

![](images/intro/drawing-fsi-partitioned-mapping.png)

vvv

## Where preCICE helps

![](images/intro/precice-features.png) 
*It's not experimental anymore.*
vvv

## What people do with preCICE (1)

<video data-autoplay width="560" height="315" >
  <source src="videos/FSI coupling for an undulation membrane tidal energy converter.mp4" type="video/mp4">
</video>

Credit: Ulrich Heck, DHCAE Tools GmbH

vvv

## What people do with preCICE (2)

<video data-autoplay width="560" height="315">
  <source src="videos/Particle impacts on flat plate with deformation (DEM+FEM).mp4" type="video/mp4">
</video>

Credit: Prasad Adhav, Univ. of Luxembourg

vvv

## What people do with preCICE (3)

<video data-autoplay width="560" height="315">
  <source src="videos/FSI coupling using OpenFOAM and preCICE for a free surface flow.mp4" type="video/mp4">
</video>

Credit: Utkan Caliskan

vvv

## In this talk

- **The preCICE library:** Couple two toy Python solvers
- **The preCICE ecosystem:** Couple OpenFOAM + deal.II

vvv

## Get the slides

<img src="images/closing/QRCode.png" style="max-height:700px;"/>

<a href="http://go.tum.de/530822">go.tum.de/530822</a>

Update required
vvv

## Organizational notes

1. You are not expected to try things live.
2. Ask questions live, feel free to interrupt me.
3. Some Live USB sticks available during the workshop
4. Find all software installed in a demo virtual machine:<br/>
<a href="https://precice.org/installation-vm.html">precice.org/installation-vm.html</a>
5. Everything presented here is free software. preCICE and all the adapters are developed publicly on GitHub: <a href="https://github.com/precice/">github.com/precice</a>
