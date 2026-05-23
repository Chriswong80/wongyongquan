---
title-slide: false
bibliography: references.bib
csl: vancouver.csl
citeproc: true
theme: serif
background-color: "#ffffff"
transition: slide
navigationMode: linear
hash: true
---

:::: {.columns}
::: {.column width="50%"}

## Sample slides
#### PlaceHolderName
#### Universiti Malaysia Perlis
#### [placeholder@email.com](mailto:placeholder@email.com)

<audio id="bg-music" src="media/audio/sb.m4a" loop></audio>

<div id="audio-credit"
     style="position: absolute; bottom: 40px; right: 20px; font-size: 0.6em; opacity: 0.6;">
  Music: “Adrift” by Scott Buckley (CC BY 4.0)
</div>

<script>
  document.addEventListener('DOMContentLoaded', () => {
    const audio = document.getElementById('bg-music');
    const credit = document.getElementById('audio-credit');

    // hide credit by default
    credit.style.display = 'none';

    const test = new Audio('media/audio/bgm.mp3');

    test.addEventListener('canplaythrough', () => {
      // bgm.mp3 exists → use it, keep credit hidden
      audio.src = 'media/audio/bgm.mp3';
    }, { once: true });

    test.addEventListener('error', () => {
      // bgm.mp3 missing → sb.m4a will play → show credit
      credit.style.display = 'block';
    }, { once: true });

    document.addEventListener('click', () => {
      if (Reveal.getIndices().h === 0) {
        audio.volume = 0.5;
        audio.play();
      }
    }, { once: true });

    Reveal.on('slidechanged', (event) => {
      if (event.indexh > 0) { audio.pause(); }
      else { audio.play(); }
    });
  });
</script>

:::

::: {.column width="50%"}
![](media/pics/logo1.png)
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide one
**Key Concepts:**
- Energy conservation per @carnot1824.
- $\Delta U = Q - W$
:::

::: {.column width="50%"}
![](media/pics/sample.png)
:::
::::

---

<span class="slide-title" data-title="My Hidden Slide Name"></span>

![](media/pics/wide.jpeg)

---

:::: {.columns}
::: {.column width="50%"}
### The Master Equation
The fundamental relation of thermodynamics:

$$\Delta U = Q - W$$

The work done $W$ is positive when the system expands against an external pressure.
:::

::: {.column width="50%"}
<video data-src="media/videos/sample.mp4" data-autoplay loop muted width="100%"></video>
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Visualizing the Gas Law
**Interactive Model:**

- P, V, and T relationships.
- Use the slider to adjust pressure.
- Observe the phase boundary.
:::

::: {.column width="50%"}
<iframe 
  data-src="media/plots/sample.html" 
  width="100%" 
  height="500px" 
  style="border:none;" 
  scrolling="no">
</iframe>
:::
::::

----------

:::: {.columns}
::: {.column width="50%"}
### Control Chart: Machine 1
**PartLength (Temperature 338, Pressure 200)**

This control chart monitors the `PartLength` for Machine 1 under the specified conditions. It helps to identify if the process is in statistical control.

:::

::: {.column width="50%"}
<img src='media/plots/control_chart_machine1_partlength.png' width='100%' style='border:none;'>
:::
::::

----------

:::: {.columns}
::: {.column width="50%"}
### Process Capability: Machine 1
**PartLength (Temperature 338, Pressure 200)**

This section presents the process capability analysis for Machine 1's `PartLength` under the specified conditions. It assesses whether the process is capable of meeting defined specifications (LSL=45, USL=55, Target=50).

:::

::: {.column width="50%"}
<img src='media/plots/capability_chart_machine1_partlength.png' width='100%' style='border:none;'>
:::
::::

----------

:::: {.columns}
::: {.column width="50%"}
### Control Chart: Machine 2
**PartLength (Temperature 338, Pressure 200)**

This control chart monitors the `PartLength` for Machine 2 under the specified conditions. It helps to identify if the process is in statistical control.

:::

::: {.column width="50%"}
<img src='media/plots/control_chart_machine2_partlength.png' width='100%' style='border:none;'>
:::
::::

----------

:::: {.columns}
::: {.column width="50%"}
### Process Capability: Machine 2
**PartLength (Temperature 338, Pressure 200)**

This section presents the process capability analysis for Machine 2's `PartLength` under the specified conditions. It assesses whether the process is capable of meeting defined specifications (LSL=45, USL=55, Target=50).

:::

::: {.column width="50%"}
<img src='media/plots/capability_chart_machine2_partlength.png' width='100%' style='border:none;'>
:::
::::

----------

:::: {.columns}
::: {.column width="50%"}
### Control Chart: Machine 3
**PartLength (Temperature 338, Pressure 200)**

This control chart monitors the `PartLength` for Machine 3 under the specified conditions. It helps to identify if the process is in statistical control.

:::

::: {.column width="50%"}
<img src='media/plots/control_chart_machine3_partlength.png' width='100%' style='border:none;'>
:::
::::

----------

:::: {.columns}
::: {.column width="50%"}
### Process Capability: Machine 3
**PartLength (Temperature 338, Pressure 200)**

This section presents the process capability analysis for Machine 3's `PartLength` under the specified conditions. It assesses whether the process is capable of meeting defined specifications (LSL=45, USL=55, Target=50).

:::

::: {.column width="50%"}
<img src='media/plots/capability_chart_machine3_partlength.png' width='100%' style='border:none;'>
:::
::::

----------

:::: {.columns}
::: {.column width="50%"}
### Process Capability: Machine 1
**PartLength (Temperature 338, Pressure 200)**

This section presents the process capability analysis for Machine 1's `PartLength` under the specified conditions. It assesses whether the process is capable of meeting defined specifications (LSL=45, USL=55, Target=50).

:::

::: {.column width="50%"}
<img src='media/plots/capability_chart_machine1_partlength.png' width='100%' style='border:none;'>
:::
::::

----------

:::: {.columns}
::: {.column width="50%"}
### Process Capability: Machine 2
**PartLength (Temperature 338, Pressure 200)**

This section presents the process capability analysis for Machine 2's `PartLength` under the specified conditions. It assesses whether the process is capable of meeting defined specifications (LSL=45, USL=55, Target=50).

:::

::: {.column width="50%"}
<img src='media/plots/capability_chart_machine2_partlength.png' width='100%' style='border:none;'>
:::
::::

----------

:::: {.columns}
::: {.column width="50%"}
### Process Capability: Machine 3
**PartLength (Temperature 338, Pressure 200)**

This section presents the process capability analysis for Machine 3's `PartLength` under the specified conditions. It assesses whether the process is capable of meeting defined specifications (LSL=45, USL=55, Target=50).

:::

::: {.column width="50%"}
<img src='media/plots/capability_chart_machine3_partlength.png' width='100%' style='border:none;'>
:::
::::

---
# Bibliography
<div id="refs"></div>
