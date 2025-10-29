---
# try also 'default' to start simple
theme: dataerai
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
title: Data Era AI
info: |
  Cornell MSE Seminar

  Learn more at [Sli.dev](https://sli.dev)
# apply UnoCSS classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
layout: center

styles:
  - './style.css'
---

# Trust, Trace, Transform: Data-Centric Materials Discovery with FPGA Inference, Kubernetes Orchestration, and Dataerai Curation

## Joshua C. Agar

### Drexel University

### Department of Mechanical Engineering and Mechanics 

#### {{ new Date().toLocaleDateString() }} 

<QrGrid :items="[
  { title: 'Slides', url: 'https://m3-learning.github.io/ISAF-PFM-Tutorial' },
]" :columns="1" />

<div class="abs-br m-6 text-xl">
  <a href="https://github.com/m3-learning" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

---
layout: default
---

# Research Philosophy
<div style="position: relative; width: 60%; max-width: 800px; aspect-ratio: 1; margin: auto;">

  <!-- Circle 1: Epitaxial Complex Oxide Synthesis -->
  <div v-click="1" style="
    position: absolute;
    top: 0;
    left: 5%;
    width: 50%;
    aspect-ratio: 1;
    border-radius: 50%;
    border: 2px solid black;
    overflow: hidden;
  ">
    <div style="
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: url('/research-philosophy/epitaxy.png') center/cover no-repeat;
      opacity: 0.5;
      z-index: 0;
    "></div>
    <div style="
      position: relative;
      top: 10%;
      width: 100%;
      text-align: center;
      font-weight: bold;
      z-index: 1;
    ">
      <h2 style="font-size: min(4vw, 20px); line-height: 1.2;">Epitaxial Complex<br>Oxide Synthesis</h2>
    </div>
  </div>

  <!-- Circle 2: Multidimensional Spectroscopy -->
  <div v-click="2" style="
    position: absolute;
    top: 0;
    left: 45%;
    width: 50%;
    aspect-ratio: 1;
    border-radius: 50%;
    border: 2px solid black;
    overflow: hidden;
  ">
    <div style="
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: url('/research-philosophy/AFM.png') center/cover no-repeat;
      opacity: 0.5;
      z-index: 0;
    "></div>
    <div style="
      position: relative;
      top: 10%;
      width: 100%;
      text-align: center;
      font-weight: bold;
      z-index: 1;
    ">
      <h2 style="font-size: min(4vw, 20px); line-height: 1.2;">Multidimensional<br>Spectroscopy</h2>
    </div>
  </div>

  <!-- Circle 3: Machine Learning -->
  <div v-click="3" style="
    position: absolute;
    top: 25%;
    left: 5%;
    width: 50%;
    aspect-ratio: 1;
    border-radius: 50%;
    border: 2px solid black;
    overflow: hidden;
  ">
    <div style="
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: url('/research-philosophy/ml.png') center/cover no-repeat;
      opacity: 0.5;
      z-index: 0;
    "></div>
    <div style="
      position: relative;
      top: 67%;
      width: 100%;
      text-align: center;
      font-weight: bold;
      z-index: 1;
    ">
      <h3 style="font-size: min(4vw, 20px); line-height: 1.2;">Machine<br>Learning</h3>
    </div>
  </div>

  <!-- Circle 4: Heterogeneous Computing -->
  <div v-click="4" style="
    position: absolute;
    top: 25%;
    left: 45%;
    width: 50%;
    aspect-ratio: 1;
    border-radius: 50%;
    border: 2px solid black;
    overflow: hidden;
  ">
    <div style="
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: url('/research-philosophy/alveo.png') center/cover no-repeat;
      opacity: 0.5;
      z-index: 0;
    "></div>
    <div style="
      position: relative;
      top: 67%;
      width: 100%;
      text-align: center;
      font-weight: bold;
      z-index: 1;
    ">
      <h2 style="font-size: min(4vw, 20px); line-height: 1.2;">Heterogeneous<br>Computing</h2>
    </div>
  </div>

</div>

---
layout: default
---

# Automated Labs

<ImageWithText
  textAbove="Reproducibility at Scale: Robots replacing grad students?"
  textBelow="Automated Labs are all the rage, but are they really useful?"
  :imageScale="0.35"
  style="margin-top: -40px"
>
  <img src="/automated-lab-introduction/automated-lab.png" alt="Automated Lab" />
</ImageWithText>

---
layout: default
---

# Ferroelectric Thin Films: Pulsed Laser Deposition

<CrossfadeImages :images="[
  'pld-schematic/PLD-Schematic-All-m2.svg',
  'pld-schematic/PLD-Schematic-All-m1.svg',
  'pld-schematic/PLD-Schematic-All.svg',
]" />

---
layout: default
---

# Ferroelectric Thin Films: Pulsed Laser Deposition

<CrossfadeImages :images="['pld-schematic/PLD-image.png']" :scale="0.8" style="margin-top: -50px" />

--- 
layout: phrases
title: "Problem"
shiftValue: left
---

## Materials Science is defined by order, periodicity, and symmetry. Can AI understand this in a meaningful way?


---
layout: default
---

# Order, Periodicity, and Symmetry

<CrossfadeImages :images="[
    'order-periodicity-symmetry.jpeg'
]" :scale="0.7" style="margin-top: -50px; margin-bottom: -60px" />

- Nature and materials science are shaped by order, periodicity, and symmetry

---
layout: default
---

# Wallpaper Group Symmetries

<CrossfadeImages :images="[
  'sym/Wallpaper-group-symmetry.svg',
]" :scale="1" style="margin-top: -80px; margin-bottom: -80px" />

- In 2D, symmetries are defined by the 17 wallpaper groups -> It is important to ask how effective are neural networks at learning symmetries from images?
- Generate a dataset with 10k total images.

---
layout: ncolumns
titleText: "Cross Validation: 10K Training Images"
columns: 3
images:
  - sym/confusion_matrix/10k train.svg
  - sym/confusion_matrix/10k valid.svg
  - sym/confusion_matrix/10k atoms.svg
titles:
  - "Training"
  - "Validation"
  - "Cross Validation"
titleClicks: [1, 2, 3]
columnWidths: [1,1,1]
textboxHeight: 20
mainHeight: 60
---


<template #text>
<div v-click="3" class="text-left">
  <ul class="list-disc pl-4" style="margin-top: -40px;">
    <li>Out of distribution cross validation fails because model cannot learn the concept of symmetry</li>
  </ul>
</div>
</template>

---
layout: ncolumns
titleText: "Cross Validation: 100K Training Images"
columns: 3
images:
  - sym/confusion_matrix/100k train.svg
  - sym/confusion_matrix/100k valid.svg
  - sym/confusion_matrix/100k atoms.svg
titles:
  - "Training"
  - "Validation"
  - "Cross Validation"
titleClicks: [1, 2, 3]
columnWidths: [1,1,1]
textboxHeight: 20
mainHeight: 60
---


<template #text>
<div v-click="3" class="text-left">
  <ul class="list-disc pl-4" style="margin-top: -40px;">
    <li>Out of distribution cross validation fails because model cannot learn the concept of symmetry</li>
  </ul>
</div>
</template>

---
layout: ncolumns
titleText: "Cross Validation: 10M Training Images"
columns: 3
images:
  - sym/confusion_matrix/10m train.svg
  - sym/confusion_matrix/10m valid.svg
  - sym/confusion_matrix/10m atoms.svg
titles:
  - "Training"
  - "Validation"
  - "Cross Validation"
titleClicks: [1, 2, 3]
columnWidths: [1,1,1]
textboxHeight: 20
mainHeight: 60
---


<template #text>
<div v-click="3" class="text-left" style="margin-top: -40px;">
  <ul class="list-disc pl-4">
    <li>10M vision transformers start to learn robust understanding of symmetry within statistical bounds of the training dataset</li>
    <li>Massive scale data not typical in materials science or chemistry is required</li>
  </ul>
</div>
</template>

---
layout: ncolumns
titleText: "Attention Map"
columns: 1
images:
  - sym/ResNet50-XCiT-AttentionMap-p4_compare.svg
titleClicks: [1]
columnWidths: [1]
textboxHeight: 20
mainHeight: 60
---

<template #col0-text>
<div class="text-center text-sm">
  Attention maps from ResNet-50 and XCiT models on "p4" symmetry inputs.
</div>
</template>

<template #text>
<div v-click="1" class="text-left" style="font-size: 0.9rem !important; line-height: 1.25; font-family: Arial, sans-serif;">
  <b>(a, f)</b> Representative input images exhibiting "p4" symmetry.  
  <b>(b–e)</b> Attention maps extracted from successive layers of the ResNet-50 model, illustrating the progression from early to deep representations.  
  <b>(g–j)</b> Attention maps generated by the XCiT model from early to deep layers, highlighting differences in feature focus.
</div>
</template>

---
layout: default
mainHeight: 40
textboxHeight: 25
---

# JPEG Compression

<CrossfadeImages :images="[
  'jpeg-compression.gif',
  'compressed-pld.jpg',
  'DCT-art.jpg'
]" :scale="0.6" style="margin-top: -80px; margin-bottom: -80px" />

- JPEG Compression: replicates images by decomposing them into a sum of basis images of the discrete cosine transform (DCT) --> There is no understanding of the image
- Neural Networks: can learn to reconstruct images from a compressed representation --> We need physics to make extrapolations from learned representations

<Reference href="https://medium.com/geekculture/how-jpeg-compression-works-a751cd877c8c" reference="Reference: How JPEG Compression Works" position="bottom" align="left" offset="20px" fontSize='12px' />

---
layout: default
---

# Physics-Informed Machine Learning

<CrossfadeImages :images="[
  'physics-informed-neural-network.png'
]" :scale="0.9" style="margin-top: -80px; margin-bottom: -80px" />

- We want to ensure parsimony of the learned representation --> Therefore we need to include physics in the learning process

<template #text>
<div class="text-left">
  <ul class="list-disc pl-4">
    <li>We want to ensure parsimony of the learned representation --> Therefore we need to include physics in the learning process</li>
  </ul>
</div>
</template>

--- 
layout: phrases
title: "Problem"
shiftValue: left
---

## Neural networks are inherently interpretive. What happens when we need high precision? How do we deal with mathematical decimation of precision?

---
layout: ncolumns
titleText: "4D-STEM: Strain Mapping"
columns: 2
images:
  - stem4d/4d-stem.png
  - stem4d/strain-shear-rotation.png
titles:
  - null
  - null
titleClicks: [1, 2]
columnWidths: [1.5, 2]
textboxHeight: 0
mainHeight: 60
roundedEdges: false
imageScale: 0.8
imageVerticalOffset: [-20, -100]
---

<template #reference>
<Reference reference="Colab: David Muller, Colin Ophus, Yimo Han, and others" position="bottom" align="left" offset="20px" fontSize='12px' />
</template>

---
layout: default
---

# 4D-STEM: Strain Mapping

<CrossfadeImages :images="[
  'stem4d/ccstae/1.png',
  'stem4d/ccstae/2.png',
  'stem4d/ccstae/3.png',
  'stem4d/ccstae/4.png',
  'stem4d/ccstae/5.png',
]" scale="0.95" style="margin-top: -20px; margin-bottom: -150px" />

<Reference reference="Colab: David Muller, Colin Ophus, Yimo Han, and others" position="bottom" align="left" offset="20px" fontSize='12px' />

---
layout: default
titleText: "4D-STEM: Strain Mapping"
mainHeight: 70
textboxHeight: 0
reference: "Colab: David Muller, Colin Ophus, Yimo Han, and others" 
---

# 4D-STEM: Strain Mapping

<CrossfadeImages :images="[
  'stem4d/simulated-data.png',
]" scale="0.85" style="margin-top: -50px; margin-bottom: -150px" />

<Reference reference="Colab: David Muller, Colin Ophus, Yimo Han, and others" position="bottom" align="left" offset="20px" fontSize='12px' />

---
layout: default
---

# 4D-STEM: Strain Mapping

<CrossfadeImages :images="[
  'stem4d/noisy-data/1.png',
  'stem4d/noisy-data/2.png',
  'stem4d/noisy-data/3.png',
]" scale="0.85" style="margin-top: -40px; margin-bottom: -150px" />

<Reference reference="Colab: David Muller, Colin Ophus, Yimo Han, and others" position="bottom" align="left" offset="20px" fontSize='12px' />

---
layout: default
---

# Improved Robustness to Background Noise

<iframe src="stem4d/mae_vs_bkg_noise_plot_enhanced.html" width="100%" height="400px" style="margin: 0;"></iframe>

<Reference reference="Colab: David Muller, Colin Ophus, Yimo Han, and others" position="bottom" align="left" offset="20px" fontSize='12px' />

---
layout: ncolumns
titleText: "4D-STEM: Strain Mapping Experimental Results"
columns: 2
images:
  - stem4d/experiment/figure-4-1.png
  - stem4d/experiment/figure-4-2.png
titleClicks: [1,2]
columnWidths: [1.5, 2]
textboxHeight: 10
mainHeight: 90
roundedEdges: false
imageScale: 0.6
imageVerticalOffset: [-100, -100]
---


<template #text>
<div v-click="2" class="text-left">
<ul class="list-disc">
  <li>The experimental results demonstrate the strain mapping capabilities of 4D-STEM, showing both the spatial distribution and magnitude of strain fields in the sample.</li>
</ul>
</div>
</template>

<template #reference>
<Reference reference="Colab: David Muller, Colin Ophus, Yimo Han, and others" position="bottom" align="left" offset="20px" fontSize='12px' />
</template>

--- 
layout: phrases
title: "Problem"
shiftValue: left
---

## Automated labs rely on preplanned trajectories and protocols. Think of trying to drive a race car with preprogrammed steering angles, throttle, and brake pedal positions -- you would almost certainly crash. Science needs control of dynamical processes at relevant time scales.

---
layout: default
---

# Ferroelectric Thin Films: Pulsed Laser Deposition

<div class="relative w-full h-90 overflow-auto">
  <img
    src="/pld-workflow/rheed-plume-highlight.png"
    class="max-w-none object-contain"
    style="transform: scale(0.60); transform-origin: top left;"
    alt="Scrollable image"
  />
</div>

---
layout: default
dragPos:
  image1: 680,95,165,400
  image2: 192,96,356,384
---

# High-Speed RHEED

<img v-drag="'image2'" src="/RHEED/Growth_mechanism-svg.svg">
<img v-click v-drag="'image1'" src="/RHEED/rheed-vertical.png">

<Reference reference="Colab: R. Ramesh, Lane Martin (Rice), John Heron (Michigan)" position="bottom" align="left" offset="20px" fontSize='12px' />


---
layout: default
mainHeight: 75
textboxHeight: 0
---

# RHEED High-Speed (>500 Hz)

<CrossfadeImages :images="[
    'RHEED/rheed-frame-grabber.png',
]" 
style="margin-top: -50px; margin-bottom: -150px" />

<template #reference>
<Reference reference="Colab: R. Ramesh, Lane Martin (Rice), John Heron (Michigan)" position="bottom" align="left" offset="20px" fontSize='12px' />
</template>

---
layout: default
titleText: "To Sand or Not to Sand, That is the Question"
mainHeight: 75
textboxHeight: 0
---

# To Sand or Not to Sand, That is the Question

<CrossfadeImages :images="[
  'plume-dynamics/plume-dynamics.png'
]" 
:scale="0.85" style="margin-top: -50px; margin-bottom: -150px" />

---
layout: ncolumns
titleText: "Structural Characterization"
columns: 2
images:
  - plume-dynamics/surface-topography.svg
  - plume-dynamics/2_RSM_Analysis.png
titles:
  - Surface Topography
  - Crystal Structure
titleClicks: [1, 2]
columnWidths: [1, 1]
textboxHeight: 30
mainHeight: 70
roundedEdges: false
imageScale: 0.8
imageVerticalOffset: [-10, -10]
---

<template #reference>
<Reference reference="Colab: R. Ramesh, Lane Martin (Rice), John Heron (Michigan)" position="bottom" align="left" offset="20px" fontSize='12px' />
</template>

---
layout: default
mainHeight: 75
textboxHeight: 0
---

# Full-Frame Plume Dynamics Imaging

<div class="h-full w-full flex items-center justify-center">
  <video controls class="max-w-full max-h-full" style="transform: scale(1.3) translateY(-10%); transform-origin: center;">
    <source src="/plume-dynamics/t5_plume_video.mp4" type="video/mp4">
  </video>
</div>

<template #reference>
<Reference reference="Colab: R. Ramesh, Lane Martin (Rice), John Heron (Michigan)" position="bottom" align="left" offset="20px" fontSize='12px' />
</template>

---
layout: default
mainHeight: 70
textboxHeight: 0
---

# Full-Frame Plume Dynamics Imaging

<CrossfadeImages :images="[
  'plume-dynamics/example-images.png',
]" scale="0.85" style="margin-top: -50px; margin-bottom: -150px"/>

<template #reference>
<Reference reference="Colab: R. Ramesh, Lane Martin (Rice), John Heron (Michigan)" position="bottom" align="left" offset="20px" fontSize='12px' />
</template>


---
layout: ncolumns
columns: 2
titleText: "Plume Dynamics Metrics"
images:
  - /plume-dynamics/4-Plume_metrics.png
  - null
titles:
 - Averaged Plume Metrics
 - null
titleClicks: [1, 2]
columnWidths: [1, 1]
textboxHeight: 0
mainHeight: 65
roundedEdges: false
imageVerticalOffset: [-100, 30]  # First image 20px from top, second image 30px from top
imageScale: 0.8
---

<template #col2>
<div v-click="2" class="text-left gap-4 flex-1 justify-start">
    <ul class="list-disc pl-4">
      <li>Computer Vision can be used to characterize the quantify the plume dynamics</li> 
      <li>There are no clear statistically significant trends in the average plume dynamics metrics</li>
    </ul>
  </div>
</template>

<template #reference>
<Reference reference="Colab: R. Ramesh, Lane Martin (Rice), John Heron (Michigan)" position="bottom" align="left" offset="20px" fontSize='12px' />
</template>


---
layout: default
titleText: "Statistical Analysis of Plume Dynamics"
mainHeight: 55
textboxHeight: 10
---

# Statistical Analysis of Plume Dynamics

<CrossfadeImages 
  :images="['plume-dynamics/5-Plume_metrics_violinplot.svg']" 
  scale="0.8" 
  style="margin-top: -50px; margin-bottom: -20px">
  <template #text>
    <li style="margin-top: -50px">Statistical distribution of the plume dynamics are bimodal, and heavy tailed for first growths</li>
  </template>
</CrossfadeImages>

---
layout: default
mainHeight: 75
textboxHeight: 0
reference: "Award: NSF 2320600: MRI: Track 2 Platform for Accessible Data-Intensive Science and Engineering" 
---

# Scaling Science, One Pod at a Time

<CrossfadeImages :images="[
  'kubernettes/kubernettes.png',
]" scale="0.8" style="margin-top: -50px; margin-bottom: -20px"/>


---
layout: default
titleText: "Kubernettes (K8s): Not a Scheduler, an Orchestrator"
mainHeight: 75
textboxHeight: 0
reference: "Award: NSF 2320600: MRI: Track 2 Platform for Accessible Data-Intensive Science and Engineering" 
---

#  K8s: Not a Scheduler, an Orchestrator

<CrossfadeImages :images="[
  'kubernettes/k8-explaination.png',
]" scale="0.8" style="margin-top: -50px; margin-bottom: -20px"/>

<div style="position: absolute; top: 50%; left: 80%;">
  <a href="https://nrp.ai/" target="_blank">
    <img v-click="1" alt="NRP Logo" src="https://nrp.ai/_astro/NRP_Horizontal_Logo.png.DQL8-3kz_19v40c.webp" class="object-cover object-center max-w-[150px] max-h-[27px] aspect-[5.56] w-full" loading="lazy">
  </a>
</div>


<Reference reference="Platform for Accessible Data-Intensive Science and Engineering" position="bottom" align="left" offset="20px" fontSize='12px' />

---
layout: default
titleText: "Timing is Everything"
mainHeight: 80
textboxHeight: 0
---

# Timing is Everything

<CrossfadeImages :images="[
    'fastml/superbowl-superbowllii.gif',
    'fastml/saquon-saquon-barkley.gif',
    ]" scale="0.8" style="margin-top: -50px; margin-bottom: -20px"/>

---
layout: default
mainHeight: 75
textboxHeight: 0
--- 

# Compact Muon Solenoid at the Large Hadron Collider

<CrossfadeImages :images="[
    'fastml/CMS-m1.png',
    'fastml/CMS.png',
    ]" scale="0.8" style="margin-top: -50px; margin-bottom: -20px"/>

<template #reference>
<Reference reference="Slide Courtesy Nhan Tran FermiLab" position="bottom" align="left" offset="20px" fontSize='12px' />
</template>

---
layout: default
titleText: "HLS4ML : Real-Time ML on FPGAs"
mainHeight: 55
textboxHeight: 0
---

# HLS4ML : Real-Time ML on FPGAs

<CrossfadeImages 
  :images="['fastml/hls4ml.jpg']" 
  scale="0.7" 
  style="margin-top: -80px; margin-bottom: -20px">
  <template #text>
      <li style="margin-top: -100px">Accessible/usable codesign workflow; open-source, targets multiple devices</li>
      <li style="margin-top: -0px">Support for reduced precision and pruning</li>
      <li style="margin-top: -0px">Spatial dataflow architectures for low latency</li>
  </template>
</CrossfadeImages>

<template #reference>
<Reference reference="Award: NSF 2320600: MRI: Track 2 Platform for Accessible Data-Intensive Science and Engineering" position="bottom" align="left" offset="20px" fontSize='12px' />
</template>

---
layout: default
mainHeight: 55
textboxHeight: 20
---

# From Static to Dynamic Control

<CrossfadeImages 
  :images="['fastml/plasma-control.gif']" 
  scale="0.8" 
  style="margin-top: -50px; margin-bottom: -20px">
  <template #text>
      <li style="margin-top: -100px">We need ML control systems to control dynamic non-equilibrium processes in materials manufacturing</li>
  </template>
</CrossfadeImages>



---
layout: default
mainHeight: 40
textboxHeight: 0
---

# From Static to Dynamic Control

<CrossfadeImages :images="[
  'fastml/plasma/GPU-version.png',
]" scale="0.9" style="margin-top: -70px; margin-bottom: -80px"/>

- Inference latency too high ($\mathcal{O}$(100 $\mu$s))
- Non-deterministic inference latency
- At least two PCIe hops ($\mathcal{O}$(1ms)) 
- Low power efficiency for remote inference

<Reference reference="Collab: Nhan Tran (FermiLabs), Giuseppe Di Guglielmo, Michael E Mauel, Gerald A Navratil (Columbia)" position="bottom" align="left" offset="0px" fontSize='8px' />

---
layout: default
mainHeight: 55
textboxHeight: 0
---

# Experimental Setup

<CrossfadeImages :images="[
  'fastml/plasma/camera-setup.png',
]" scale="0.7" style="margin-top: -70px; margin-bottom: -50px"/>

- Two Phantom Vision cameras capable of 100,000 fps
- Direct optical imaging of tokamak plasma
<Reference reference="Collab: Nhan Tran (FermiLabs), Giuseppe Di Guglielmo, Michael E Mauel, Gerald A Navratil (Columbia)" position="bottom" align="left" offset="0px" fontSize='8px' />

---
layout: default
titleText: "FPGA Block Diagram"
mainHeight: 55
textboxHeight: 0
reference: "Collab: Nhan Tran (FermiLabs), Giuseppe Di Guglielmo, Michael E Mauel, Gerald A Navratil (Columbia)"
---

# FPGA Block Diagram

<CrossfadeImages :images="[
  'fastml/plasma/camera-setup-2.png',
]" scale="0.7" style="margin-top: -70px; margin-bottom: -50px"/>

- Data is aquired over CoaXPress --> Custom Logic ML Inference --> FPGA --> Control Signals

<Reference reference="Collab: Nhan Tran (FermiLabs), Giuseppe Di Guglielmo, Michael E Mauel, Gerald A Navratil (Columbia)" position="bottom" align="left" offset="0px" fontSize='8px' />

---
layout: ncolumns
titleText: "Timing and Synchronization"
columns: 2
images:
  - fastml/plasma/tokamak-plasma-timing.png
  - null
titleClicks: [1, 2]
columnWidths: [1, 1]
textboxHeight: 0
mainHeight: 70
roundedEdges: false
---

<template #col2>
<div v-click="2" class="text-left gap-4 flex-1 justify-start">
    <ul class="list-disc pl-4">
      <li>1. 0.3 ns single CPU clock cycle</li>
      <li>2. 0.1-0.2 μs reading 1 MB block from RAM </li>
      <li>3. 0.1-0.5 μs PCIe hop</li>
      <li>4. 100 μs – 1 ms reading 1 MB block from NVMe</li>
      <li>5. 0.1 ms – 1 ms local network ping</li>
      <li>6. 10 ms – 20 ms reading 1 MB block from spinning disk </li>
    </ul>
  </div>
</template>

<template #reference>
<Reference reference="Collab: Nhan Tran (FermiLabs), Giuseppe Di Guglielmo, Michael E Mauel, Gerald A Navratil (Columbia)" position="bottom" align="left" offset="0px" fontSize='8px' />
</template>

---
layout: default
titleText: "FPGA Block Diagram"
mainHeight: 60
textboxHeight: 0
---

# FPGA Codesign Optimization

<CrossfadeImages :images="[
  'fastml/plasma/pareto.svg',
]" scale="0.7" style="margin-top: -70px; margin-bottom: -50px"/>

- How do you efficiently achieve a good tradeoff between latency (power), and accuracy?

<Reference reference="Collab: Nhan Tran (FermiLabs), Giuseppe Di Guglielmo, Michael E Mauel, Gerald A Navratil (Columbia)" position="bottom" align="left" offset="0px" fontSize='8px' />


---
layout: main-custom-layout
titleText: "Neural Architecture Search for FastML on FPGAs"
mainHeight: 70
textboxHeight: 0
---

<CrossfadeImages :images="[
  'fastml/FastML-NAS.png',
]"/>

---
layout: ncolumns
titleText: "DataFed TorchFlow"
columns: 2
images:
  - fastml/torchlogger/datafedTorchflow.png
  - null
titleClicks: [1, 2]
columnWidths: [1, 1]
textboxHeight: 0
mainHeight: 55
reference: "Colab: Jane Greenberg (Drexel University)"
roundedEdges: false
---

::col1::
## What Does DataFed TorchFlow Do?

- Preserves script with a checksum.
- Maintains a copy or reference to the training data.
- Extracts the neural network model graph.
- Extracts the optimizer state and hyperparameters.
- Records the Python and hardware environment.
- Allows the addition of any custom metadata.

::text::
- <span v-click="3">Pip installable python package `pip install datafed_torchflow`</span>
- <span v-click="3">With a single instantiation provides a drag-and-drop replacement for `model.save()` in PyTorch</span>

---
layout: main-custom-layout
titleText: "Future Activities: Dose Control in Electron Microscopy"
mainHeight: 70
reference: "Colab: Seda Ogrenci (Northwestern), David Flannigan (Minnesota)"
textboxHeight: 0
---

<CrossfadeImages :images="[
  'fastml/EM.png',
]"/>

---
layout: main-custom-layout
titleText: "Acknowledgements"
mainHeight: 83
textboxHeight: 0
---

<CrossfadeImages :images="[
  'people.png',
]"/>

---
layout: main-custom-layout
titleText: "Source Materials"
mainHeight: 83
textboxHeight: 0
---

<QrGrid :items="[
  { title: 'Slides', url: 'https://m3-learning.github.io/Brookhaven-national-lab-8-18-2025/1' },
  { title: 'DataFed', url: 'https://datafed.ornl.gov/ui/welcome' },
  { title: 'Learning Symmetries', url: 'https://github.com/yig319/Understanding-Experimental-Images-by-Identifying-Symmetries-with-Deep-Learning' },
  { title: 'RHEED Analysis', url: 'https://github.com/m3-learning/Predicting-Pulsed-Laser-Deposition-SrTiO3-Homoepitaxy-Growth-Dynamics-using-RHEED'},
  { title: 'Plume Dynamics', url: 'https://github.com/m3-learning/SrRuO3_Plume_Dynamics'},
  { title: 'Auto4DSTEM', url: 'https://github.com/m3-learning/Auto4DSTEM'},
  { title: 'Embedding Visualizer', url: 'https://github.com/chirayupatel9/embedding-be-lmdb'},
  { title: 'HLS4ML', url: 'https://fastmachinelearning.org/hls4ml/'},
  { title: 'FastML Tutorial Medium', url: 'https://medium.com/@forelliryan/deploying-neural-networks-for-in-situ-inference-on-frame-grabber-fpgas-in-high-speed-imaging-6201557fdabc'},
]" :columns="5" />
