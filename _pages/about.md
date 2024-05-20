---
layout: about
title: Dylan R. Schlichting
permalink: /
description:

profile:
  align: right
  image: prof_pic_NM.jpg
  address: >
    <p>TA-03 200, Los Alamos National Laboratory</p>
    <p>Los Alamos, NM 87545</p>

news: false  # includes a list of news items
selected_papers: true # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---

I'm a PhD candidate in the [Oceanography](https://ocean.tamu.edu/) Department at Texas A&M University advised by [Dr. Rob Hetland](https://hetland.github.io/publications/) and recently defended my dissertation! I'm also an [SCGSR](https://science.osti.gov/wdts/scgsr) fellow at Los Alamos National Laboratory (LANL) that works with Drs. [Mark Petersen](https://mark-petersen.github.io/home/) and [Katherine Smith](https://www.linkedin.com/in/katherine-smith-6155bbb6/). My research at TAMU focused on characterizing mixing processes within the estuary-river plume continuum. I spent several years thinking about so called "numerical mixing", which is a type of spurious mixing that arises in ocean models as a consequence of representing the bulk transport of tracers by currents with discrete approximations. We looked at numerical mixing in idealized and realistic numerical simulations of the Texas-Louisiana (TXLA) shelf in the northern Gulf of Mexico. My work at LANL is a change of pace and has focused on assessing the capabilities of the DOE's global ocean model [MPAS-O](https://mpas-dev.github.io/) in representing coastal processes, using the TXLA shelf as a case study.

I'm looking to start a postdoctoral position in August 2024!

I received my bachelor's degree in civil engineering from the University of Maine in December 2019. My journey into physical oceanography started in May 2017 when Drs. [Kimberly Huguenard](https://civil.umaine.edu/faculty/kimberly-huguenard/) and [Brandon Lieberthal](https://scholar.google.com/citations?user=Hi7W6iMAAAAJ&hl=en) hired me as a research assistant at the end of my first year. We worked on several observational and modeling-based coastal engineering projects, including: 1) [Sensing Storm Surge](http://sensingstormsurge.acg.maine.edu/), which established a citizen science program in several Maine estuaries, rivers, and harbors, 2) quantifying the environmental impacts of coastal armoring structures on beach profiles in Saco Bay, ME, 3) and testing the feasibility of suspended kelp farms as a solution to coastal erosion with analytical modeling, and 4) quantifying the hydrodynamic impact of floating oyster farms in a wave tank.

During my second year, I was fortunate to be accepted into TAMU's "Observing the Ocean" Research Experience for Undergraduates (REU) program, which is funded by the National Science Foundation. That summer, I met Dr. Hetland and gained experience working with ROMS model output of Copano Bay, which is an estuary on the Texas coast. Within the first few weeks I made an important realization -- I wanted to be a physical oceanographer, not an engineer. I was more drawn to questions like "Why is the salinity structure in this estuary so difficult to get right with a model?" rather than "How much faster will a new coastal armoring structure erode the beach?". However, for many estuaries and coastal regions, these types of questions are inextricably linked.

My REU studies heavily influenced the types of questions I found myself chasing at the start of my PhD. It also led to a coauthored paper in *JPO* that focuses on developing simple approximations to estuarine mixing using the idea of mixing pathways, which is the mixing a water mass experiences during its flow pathway.

I started my PhD in Jan. 2020, just before the Covid-19 pandemic began. I'm part of the NSF-NERC [SUNRISE](https://sunrise-nsf.github.io/) project, which seeks to understand the interactions between near-inertial motions, submesoscale proceses, and their local impacts on turbulent (physical) mixing. Numerical models are powerful tools for studying ocean mixing, however, they are prone to numerical issues because they represent physical processes with discrete approximations. Numerical mixing is one such error; the process by which the discretized transport of tracers by currents results in spurious mixing. Numerical mixing can introduce biases in numerical models and cause them to drift away from reality. This is different than what modelers often call physical mixing. That is, the mixing based on physical conservation laws. We have a paper that quantifies numerical mixing in the TXLA model in *JAMES*, which is the first chapter of my dissertation. The second chapter used the lessons learned from this first paper to better understand the impacts of that mixing on the larger-scale ocean circulation and tracer state.  

My work at LANL is much more applied. The research question can be summarized as: "Can a global ocean model with a regionally refined mesh represent coastal ocean processes with similar fidelity to regional-scale models?" This work is important because coastal communities are and will continue to be adversely affected by climate change. However, coastal processes are poorly represented in climate models because they occur at scales of motion that are smaller than most climate models can resolve. Climate models require awesome computational resources. A standard laptop has around 4-16 cores and a 1TB internal hard drive. Climate models that don't even resolve coastal processes often require thousands of cores to run and are capable of producing Petabytes ($$\mathcal{O}$$(1000 TB)) of output.

My project essentially stress-tests the DOE's global ocean model [MPAS-O](https://mpas-dev.github.io/) by turning up the resolution over the TXLA shelf. The idea is to compare it with regional-scale models like [ROMS](https://www.myroms.org/), which are run at much higher resolution but for smaller domains. ROMS is designed to simulate these types of processes, MPAS-O is not. The results of this project can be used to improve climate models and thus are ability to understand the ocean's complex relationship with climate and weather.

Here is a link to my <a href='/_pages/CV.pdf' class='image fit'> CV</a>.

#### Research Interests
---
1. Numerical/spurious mixing
2. Coastal ocean submesoscale processes
3. Water mass transformation techniques
4. Estuarine exchange flow and mixing
5. Open science

#### Education
---
* PhD. in Oceanography, Texas A&M University, (Expected Aug. 2024)
* B.S. in Civil Engineering, University of Maine, (Dec. 2019)
  * Minor in Mathematics

#### Publications
---
5. Wei Hsu, F., **Schlichting, D.**, Shearman, R.K., Nash, J.D., Kobashi, D., Hetland, R.D. Near-Resonance between Shelf Ocean and Semidiurnal Atmospheric Tidal Wind. *Journal of Physical Oceanography*. Submitted.

4. **Schlichting, D.**, Hetland, R., \& Jones, S. Numerical mixing suppresses submesoscale baroclinic instabilities over sloping bathymetry. *Journal of Advances in Modeling Earth Systems*. In-revision.

3. **Schlichting, D.**, Qu, L., Kobashi, D, and Hetland, R. D. (2023). Quantification of physical
and numerical mixing in a coastal ocean model using salinity variance budgets. *Journal
of Advances in Modeling Earth Systems*, 15, e2022MS003380. [https://doi.org/10.1029/2022MS003380](https://doi.org/10.1029/2022MS003380).

2. Qu, L., Hetland, R. D., & **Schlichting, D.** (2022). Mixing pathways in simple box models. *Journal of Physical Oceanography*. [https://doi.org/10.1175/JPO-D-22-0074.1](https://doi.org/10.1175/JPO-D-22-0074.1).

1. Spicer, P., **Schlichting, D.**, Huguenard, K., Roche, A., and Rickard, L. (2021). Sensing Storm Surge: A framework for establishing a citizen scientist monitored water level network. *Ocean and Coastal Management*, 211, 105802. [https://doi.org/10.1016/j.ocecoaman.2021.105802](https://doi.org/10.1016/j.ocecoaman.2021.105802).
{: reversed="reversed"}

#### Personal Interests
Outside of work, I enjoy running, hiking, and strength training. Since I moved to New Mexico, I spend most of my free time outdoors. See the [photo gallery](/gallery/) page for some pictures I've accumulated over the years.
