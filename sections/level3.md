# Using the preCICE ecosystem

Example: Coupling OpenFOAM and CalculiX

---

## The big picture

<img data-src="images/intro/precice-overview-0.svg" style="border:none; box-shadow:none; max-width:80%;">

Notes:
- We will do an "adpated code", no adapter

vvv

## The big picture

<img data-src="images/intro/precice-overview-1.svg" style="border:none; box-shadow:none; max-width:80%;">

vvv

## The big picture

<img data-src="images/intro/precice-overview-2.svg" style="border:none; box-shadow:none; max-width:80%;">


---

## What does the adapter do?

<img src="images/level2/openfoam_adapter_overview_linking.svg" />

vvv

## What does the adapter do?

<img src="images/level2/openfoam_adapter_overview_data.svg" />

vvv

## What does the adapter do?

<img src="images/level2/openfoam_adapter_overview_checkpointing.svg" />

vvv

## What does the adapter do?

<img src="images/level2/openfoam_adapter_overview_timestep.svg" />

---

![](images/level3/quickstart.png)

---

## Tutorial: Channel with a perpendicular flap

<img src="images/level3/flap_perp.png" style="max-height:400px;"/>

<small>Find this tutorial on <a href="https://precice.org/tutorials-perpendicular-flap.html">precice.org/tutorials-perpendicular-flap.html</a>.</small>

vvv

## Arbitrary solver combinations

| FLUID             | SOLID                  |
| ---               | ---                    |
| pimpleFoam        | CalculiX               |
| SU2               | deal.II                |
| Nutils            | FEniCS                 |
|                   | DUNE                   |
|                   | solidDisplacementFoam  |
|                   | solids4Foam            |

vvv

## Arbitrary solver combinations

<img src="images/level3/perpendicular-flap-comparison.png" style="max-height:400px;"/>

<small>Note: SU2 models a compressible fluid, OpenFOAM and Nutils an incompressible one.</small>

vvv

## Dependencies

- [preCICE](https://precice.org/installation-overview.html) v2 (e.g. [packages for Ubuntu](https://github.com/precice/precice/releases))
- Recent OpenFOAM (e.g., v2306)
- [OpenFOAM-preCICE adapter](https://precice.org/adapter-openfoam-overview.html) v1
- [CalculiX](http://calculix.de/) 2.20
- [CalculiX-preCICE adapter](https://precice.org/adapter-calculix-overview.html) 2.20.0

---

## File structure

```
- precice-config.xml
- fluid-openfoam/
    - 0/U ...
    - constant/dynamicMeshDict ...
    - system/
      - controlDict
      - preciceDict
    - ...
- solid-calculix/
    - flap.inp
    - config.yml
    - ...
```

vvv

## For demonstration purposes

- In `precice-config.xml`:
    - Reduce the `max-time` from 5s to 1.5s
    - Switch to a serial-explicit coupling scheme
- In `solid-calculix/flap.inp`:
    - Lower the solid density from 3000 to 30
