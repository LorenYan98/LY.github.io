---
title: "DesignCheck2, Mar.08.2021"
excerpt: "**The project aims to form a systematic check for a W section element**<br/><img src='/LY.github.io/images/designcheck.png' width='40%' height = '40%'>"
collection: portfolio
---

2021 Spring Made by **Peidong Yan** Directed by **R.Chana**. 

[Design Check sample output](https://lorenyan98.github.io/LY.github.io/files/DesignCheck2.Structural.CombinedBeamChecks.pdf)

**DesignCheck is a standard framework for writing engineering calculations in code**. The W-section DesignCheck is a C# framework I authored that aims to provide the simplest way to compute a systematic check for a W section element in accordance with Canadian Code CSA S16-14, one-click with a full calculation report. 

This project will be contributing to a central store of Arup knowledge that will be useful forever.

* Prgramming language: C#
* Platform: Visual Studio Code, Gitlab  

User input
---
The code requires the user to input section properties and loading condition along the major and minor axis. Detailed explaination for each variable will be automatically displayed when the cursor points to it.

<img src='/LY.github.io/images/designsc.png'>

DesignCheck Methodology (Partial Flowchat)
---

The code reads through user's input and select proper check based on it.
* _S16-14 11.3, 11.2_, Section Classification 
* _S16-14 13.3_, Compression
* _S16-14 13.2_, Tension
* _S16-14 13.4_, Shear
* _S16-14 13.5, 13.6_, Bending, Biaxial Bending
* _S16-14 13.3, 13.8_, Compression + Bending (Calculation varies upon differet section classes)
    * Cross section check
    * Overall check
    * Lateral torsional buckling check
* _S16-14 13.9_, Tension + Bending (Calculation varies upon differet section classes)

<img src='/LY.github.io/images/flowchart.png'>

