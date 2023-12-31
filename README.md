
<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/NiyoushaRahimi/Data-Guided-Regulator-for-Adaptive-Nonlinear-Control">
  </a>

  <h3 align="center">Data Guided Regulator for Adaptive Nonlinear Control</h3>

  <p align="center">
    Niyousha Rahimi, RAIN Lab University of Washington
    <br />
    <a href="#usage">View Demo</a>
    ·
    <a href="">Report Bug</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      </li>
      <li>
      <a href="#Requirements">Requirements</a></li>
      </ul>
    </li>
    <li><a href="#main-project">Main Project</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#Citing">Citing</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project
* Code will be updated
* This project is the implementation of this [paper](https://).

### Abstract
This paper addresses the problem of designing a data-driven feedback controller for complex nonlinear dynamical systems in the presence of  time-varying disturbances with unknown dynamics. Such disturbances are modeled as the <b class="term">unknown</b> part of the system dynamics. The goal is to achieve finite-time regulation of system states through direct policy updates while also generating informative data that can subsequently be used for data-driven stabilization or system identification. 

First, we expand upon the notion of <b class="keywords">regularizability</b> and characterize this system characteristic for a linear time-varying representation of the nonlinear system with locally-bounded higher-order terms. <b class="keywords">Rapid-regularizability</b> then gauges the extent by which a system can be regulated in finite time, in contrast to its asymptotic behavior.

We then propose the <b class="keywords">DG-RAN</b> algorithm, an online iterative synthesis procedure that utilizes discrete time-series data from a single trajectory for regulating system states and identifying disturbance dynamics. The effectiveness of our approach is demonstrated on a 6-DOF power descent guidance problem in the presence of adverse environmental disturbances.

* The quadratic funnel computed by the $\gamma$-iteration for the 6-DOF power descent problem in the presence of unmodeled time-varying disturbances. The initial condition of each test case was randomly sampled from the funnel entry, and the system uses only the offline robust controller.




<div style="text-align: center;">
    <img src="/Figures/state_space_funnel_with_disturbance_v2.png" width="500">
    <p><b class="keywords">Fig 1. (a)</b> position and linear velocity in state space $\mathcal{E}_Q$</p>
</div>

<div style="text-align: center;">
    <img src="/Figures/tw_state_space_funnel_with_disturbance_v2.png" width="500">
    <p><b class="keywords">Fig 1. (b)</b> rotation angles and angular velocity in state space $\mathcal{E}_Q$</p>
</div>


* State trajectories generated using the online DG-RAN algorithm for the 6-DOF power descent problem in the presence of unmodeled time-varying disturbances. The initial condition for this test case was randomly sampled from the funnel entry, and the proposed method was implemented online for each test case. The shaded gray area represents $\mathcal{E}_{\bar{Q}(t)}$ projected onto each state, and the shaded dark blue area represents the projection of the inner invariant funnel $\mathcal{E}(t)$ onto each state.


<div style="text-align: center;">
    <img src="/Figures/rv_disturbance_v2.png" width="500">
    <p><b class="keywords">Fig 2. (a)</b> position and linear velocity in state space $\mathcal{E}_Q$</p>
</div>

<div style="text-align: center;">
    <img src="/Figures/tw_disturbance_v2.png" width="500">
    <p><b class="keywords">Fig 2. (b)</b> rotation angles and angular velocity in state space $\mathcal{E}_Q$</p>
</div>

## Requirements

The main requirements are as follows:
* --

* GPU and processor I used:
    <ul>
      <li>Intel(R) Core(TM) i7-8850H CPU @  2.60 GHz, 2592 Mhz, 6 Core(s),  12  Logical Processor(s) </li>
      <li>Nvidia Quadro P2000</li>
    </ul>




## Main project

* The main project is carried out in main.py.








<!-- USAGE EXAMPLES -->
## Usage
Here's a demo of the simulation in <b class="keywords">Unreal Engine</b>:



<!-- CONTACT -->
## Contact

Niyousha Rahimi - nrahimi@uw.edu

RAIN Lab, University of Washington


## Citing

If you use any part of the code, kindly cite the following associated publication.

```
@inproceedings{rahimi2024data,
  title={Data-Guided Regulator for Adaptive Nonlinear Control},
  author={Rahimi, Niyousha and Mesbahi, Mehran},
  booktitle={AIAA SCITECH 2024 Forum},
  pages={},
  year={2024}
}
```

## Acknowledgements
The research of the first author has been partially supported by the UW+Amazon Science Hub Fellowship. This research has also been supported by NSF grant ECCS-2149470.



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/newsha-rahimi/
[product-screenshot]: images/screenshot.png
