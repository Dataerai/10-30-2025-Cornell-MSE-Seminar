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
reference: 
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
  - stem4d/experiment/figure-4-1.svg
  - stem4d/experiment/figure-4-2.svg
titleClicks: [1,2]
columnWidths: [1.5, 2]
textboxHeight: 10
mainHeight: 55
roundedEdges: false
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
layout: ncolumns
titleText: "High-Speed RHEED Results"
columns: 2
images:
  - RHEED/Growth_mechanism-svg.svg
  - RHEED/rheed-vertical.png
titleClicks: [1, 2]
columnWidths: [1, 1]
textboxHeight: 0
mainHeight: 70
roundedEdges: false
---

<template #reference>
<Reference reference="Colab: R. Ramesh, Lane Martin (Rice), John Heron (Michigan)" position="bottom" align="left" offset="20px" fontSize='12px' />
</template>

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
  'plume-dynamics/plume-dynamics.png',
]" 
scale="0.85" style="margin-top: -50px; margin-bottom: -150px" />

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
textboxHeight: 0
mainHeight: 70
roundedEdges: false
---


<CrossfadeImages :images="[
  'plume-dynamics/surface-topography.svg',
  'plume-dynamics/2_RSM_Analysis.png'
]" scale="0.9"/>

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
images:
  - plume-dynamics/4-Plume_metrics.png
  - null
titles:
 - Averaged Plume Metrics
 - null
titleClicks: [1, 2]
columnWidths: [1, 1]
textboxHeight: 0
mainHeight: 65
roundedEdges: false
---

# Plume Dynamics Metrics

<template #col1>
<div v-click="2" class="text-left gap-4 flex-1">
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

<CrossfadeImages :images="[
  'plume-dynamics/5-Plume_metrics_violinplot.svg',
]" />

::text::
- Statistical distribution of the plume dynamics are bimodal, and heavy tailed for first growths

---
layout: default
titleText: "Heatmap of Plume Area"
mainHeight: 55
textboxHeight: 10
---

<CrossfadeImages :images="[
  'plume-dynamics/5_Plume_Area_Heatmap.png',
]" />

::text::
- Heatmaps of plume area show anomalous behavior close to edge of the target