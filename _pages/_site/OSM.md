<!-- ---
layout: page
title: ocean sciences meeting
permalink: /Ocean Sciences/
description:
nav: true
---
This page contains supplemental material for my 2022 Ocean Sciences Presentation. A copy of the slides may be found <a href='/_pages/osm_slides.pdf' class='image fit'> here</a>. If you're interested in the math used to derive the equations for salt squared $$s^2$$, salt anomaly squared $$s^{\prime^2}$$, and their differences, check out <a href='/_pages/numerical_mixing_differences.pdf' class='image fit'> this document</a>.

Both budgets may be used to quantify the bulk physical mixing within a control volume, defined as the destruction of salinity variance $$\chi$$. Recent work by MacCready et al. (2018, JPO) and Burchard et al. (2019, JPO) suggests that the numerical mixing can be quantified as the residual of each budget, however since they are different equations they will yield different estimates of numerical mixing when calculated offline. The second document walks through the accompanying math in detail. The $$s^{\prime^2}$$ approach is often defined as the salinity variance and gives a closer representation of the true numerical mixing created by the advection scheme (we use MPDATA), however the $$s^2$$ budget is easier to apply to observations and model output because the salinity isn't referenced to an averaged value (often the volume average). If you calculate the numerical mixing online, this is not an issue.

The key equation that describes the numerical mixing from the $$s^2$$ budget in terms of $$s^{\prime^2}$$ is:
$$
\begin{equation}
M_{num, s^2} = -\frac{d \overline{s}^2}{d t} V   - 2\overline{s} \iiint_V \frac{\partial s^\prime}{\partial t} \, dV - \overline{s}^2 \iint_A \textbf{u} \cdot \, d\textbf{A} -
    2 \overline{s} \iint_A (\textbf{u}s^{\prime}) \cdot \, d\textbf{A}  +\\
    \iint_A (2\overline{s}^2+2 \overline{s} s^\prime)(E-P) \, dA - M_{num, s^{\prime^2}},
\end{equation}
$$
so we can see that there a number of extra terms that must be considered to properly compare the numerical mixing estimates. -->
