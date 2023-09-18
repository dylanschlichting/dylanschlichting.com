---
layout: page
title: projects
permalink: /projects/
description:
nav: true
---
I use Regional Ocean Modeling System ([ROMS](https://www.myroms.org/)) as part of the Coupled-Ocean-Atmosphere-Wave-Sediment Transport model ([COAWST](https://www.usgs.gov/centers/whcmsc/science/coawst-a-coupled-ocean-atmosphere-wave-sediment-transport-modeling-system)) to make numerical simulations of the coastal ocean. ROMS has been a primary tool for the estuarine and coastal modeling community since the 1990s. Check out some of my projects below. The first two project images are linked to youtube videos because they are too large to host on GitHub.

### High-resolution modeling of the Texas-Louisiana shelf
[![Here](txla_mnum_surf_1011.jpg)](https://www.youtube.com/watch?v=ZLfN9I5l6tw)

The TXLA model domain covers much of the northern Gulf of Mexico out to the outer continental slope. The current version of the model was developed by Dr. <a href="https://www.researchgate.net/profile/Daijiro-Kobashi">Daijiro Kobashi</a> to study submesoscale processes in the upper ocean for the SUNRISE project. The animation shows a two-way nested simulation, where inside the black box the horizontal resolution is increased by a factor of five. Two-way nesting means that the coarse (parent) and fine (child) grids are allowed to exchange information across the open boundary.

During summer, the regional diurnal land-sea breeze interacts with freshwater forcing from the Mississippi and Atchafalaya Rivers. These interactions cause a rich submesoscale eddy field with strong inertial currents to develop. This can be seen in plots of the surface relative vorticity $$(\partial_x v - \partial_y u) / f$$ as shown in subplot (a). Here, subscripts denote partial differentiation. These eddies have sharp, energetic fronts, which are marked by positive (red) values. The fronts have strong lateral salinity gradients ($$\nabla_h s$$) as shown in subplot (b). Subplot (c) shows a normalized version of the frontogenesis function (Hoskins, 1982), which tells us whether those salinity gradients are being sharpened by frontogenesis or destroyed by frontolysis. The fronts are thought to be hotspots for numerical mixing, a type of spurious (i.e., numerically-induced) mixing that can degrade the accuracy of numerical models. This is because the model must discretize very large changes in salinity over a small distances, which can decrease the fidelity of a numerical solver. The video shows that numerical mixing (subplot (d)) can greatly exceed the mixing based on physical conservation laws (subplot (e)) at shallow depths.

### Numerical mixing in an idealized coastal shelf model
[![Here](shelf_advschemes_zerop1pa.jpeg)](https://www.youtube.com/watch?v=NW_Qem0l8EY)

One of the reasons we use idealized modeling is to build intuition. In the real ocean, many mixing processes occur simultaneously, spanning over eight orders of magnitude in space and time. An idealized model allows us to perturb individual processes like how fast the wind blows over the ocean surface while keeping everything else constant. Here, we use an idealized coastal ocean model that develops a *submesoscale* eddy field to investigate how numerical mixing impacts the larger scale flow and salinity field.

The term submesoscale refers to ocean processes spanning approximately 100 m - 10 km in space, although they are better defined by their dynamical characteristics. Manifesting primarily as fronts, filaments, and eddies, submesoscales have $$\mathcal{O}(1)$$ Rossby numbers. A flow's Rossby number represents the ratio of the inertial force to the Coriolis force. Mathematically, this can be represented as $$Ro=U/fL \sim \zeta/f$$, where $$U$$ is a characteristic velocity scale, $$f$$ is the Coriolis parameter, and $$L$$ is a characteristic length scale. This is approximately equal to the relative vorticity $$\zeta/f$$. As the Rossby number approaches unity, it implies the flow is becoming more ageostrophic and three-dimensional. Classical approximations such as geostrophy, quasi-geostrophy, and semi-geostrophy break down as $$Ro$$ increases. 

The video show the development of the eddy field after several days. An oscillatory along-shore wind stress is applied after four days to energize the fronts and increase numerical mixing. Each column shows a numerical simulation with a different tracer advection scheme. These are just different numerical methods for solving the tracer conservation equation in ROMS. By the end of the video, the larger scale salinity field is generally the same between schemes. However, we can see that MPDATA has the most small-scale structure within the anticyclones but HSIMT has smoother fronts.

### Storm surge in estuaries
  <img src = "../_pages/sss_combined.png" alt="surge"> <br>
During my undergrad, I worked on the Sensing Storm Surge Project, which investigated storm surge in several Maine estuaries. I helped set up and maintain the citizen science network. The first picture is me prepping a mooring in Bass Harbor. The figure to the right is modified from Spicer et al. (2021), our Ocean and Coastal Management publication that shows observed surge in two estuaries. The figure demonstrates the effects of channel convergence on surge height.
