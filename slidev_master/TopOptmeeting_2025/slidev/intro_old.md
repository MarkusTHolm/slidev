## **Architected materials** -- Applications
<p> </p>



- Enabled by additive manufacturing
- Metals and polymers

- <span v-mark.orange.v-mark="1"> Aerospace, </span> <span v-mark.orange.v-mark="2"> orthopedic implants, </span> <span v-mark.orange.v-mark="3"> sporting gear </span>, etc.


<div v-click="4">

- Active research field

</div v-click>

<div v-click="1">
<img src="/media/MetalAm/ssm-slm-inconel-sparrow.png" style="position:fixed; bottom:80px; left:-40px; width:325px"/>
<p style="position:fixed; bottom:50px; left:40px; text-align:left; font-weight: lighter"> <sup>1)</sup> </p> 
</div v-click>

<div v-click="1"> 
<img src="/media/MetalAm/ESAbracket.png" style="position:fixed; bottom:90px; right:350px; width:375px"/>
<p style="position:fixed; bottom:100px; right:615px; text-align:left; font-weight: lighter"> <sup>2)</sup> </p>  
</div v-click> 

<div v-click="2">
<img src="/media/MetalAm/part1.png" style="position:fixed; bottom:100px; left:590px; width:800px"/>
<p style="position:fixed; top:215px; left:685px; text-align:left; font-weight: lighter"> <sup>3)</sup> </p>   

<img src="/media/MetalAm/part2.png" style="position:fixed; bottom:290px; left:680px; width:200px"/>

<img src="/media/MetalAm/part3.png" style="position:fixed; bottom:95px; left:270px; width:600px"/>
</div v-click>

<div v-click="3">
<img src="/media/Carbon/addidas.png" style="position:fixed; bottom:0px; right:270px; width:250px"/>
<p style="position:fixed; bottom:40px; right:515px; text-align:left; font-weight: lighter"> <sup>4)</sup> </p>  

<img src="/media/Carbon/riddel_helmet.png" style="position:fixed; bottom:20px; right:20px; width:250px"/>
<p style="position:fixed; bottom:40px; right:250px; text-align:left; font-weight: lighter"> <sup>5)</sup> </p>
</div v-click>

<Footnotes separator>
  <div v-click="1">
  <Footnote :number=1> all3dp.com </Footnote>
  </div v-click>

  <div v-click="1">
  <Footnote :number=2> jawstec.com </Footnote>
  </div v-click>

  <div v-click="2">
  <Footnote :number=3> Solar Orbiter Sun Sensor Bracket (ESA) </Footnote>
  </div v-click>

  <div v-click="3">
  <Footnote :number=4> Carbon - Adidas </Footnote>
  </div v-click>

  <div v-click="3">
  <Footnote :number=5> Carbon - Riddel </Footnote>
  </div v-click>

</Footnotes> 


<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />

<!--
- Motivation: Lightweighting and tailored properties, and perhaps even better

- Motivate why fracture properties are important
-->

---

## **Architected materials** -- Properties
<p> </p>
  

<div class="grid grid-cols-2 gap-4">
  <div>
    Tailor stiffness 
    <img src="/media/ashby/g23.png" style="width:600px"/>
    <p style="position:relative; top:-10px; right:0px; text-align:right"> <sup>1)</sup> </p>  
  </div>
  
  <div>
    Tailor, and improve fracture toughness?
    <img src="/media/ashby/image1-3.png" style="width:390px"/>
    <p style="position:relative; top:-10px; right:40px; text-align:right"> <sup>2)</sup> </p>  
  </div>

</div>

<Footnotes separator>
  <Footnote :number=1> Jenett et al. (2017) </Footnote>
  <Footnote :number=2> Inspired by Tankasala et al. (2015) </Footnote>
</Footnotes> 

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />

---
layout: two-cols-header
---

## **Methods** -- Periodic structures

<p> </p>

::left::

- Crack will see repeating patterns
- Linear homogenization theory to impose constraints on $\mathbf{C}^H$:
$$
\begin{bmatrix} 
\sigma_{11} \\
\sigma_{22} \\
\sigma_{12} \\
\end{bmatrix}
=
\underbrace{
\begin{bmatrix} 
C_{11} & C_{12} & C_{13} \\
C_{21} & C_{22} & C_{23} \\
C_{31} & C_{32} & C_{33} \\
\end{bmatrix}
}_{\mathbf{C}^H}
\begin{bmatrix} 
\epsilon_{11} \\
\epsilon_{22} \\
\epsilon_{12} \\
\end{bmatrix}
$$

- Basis cell to unit cell

<img src="/media/figures/fig1_homogenization.svg" style="position:relative; width:400px; bottom:20px; left:50px"/>

::right::


<div v-click> 

- 4 different crack configurations:
<img src="/media/figures/cracks_Nbc_3.svg" style="position:relative; width:400px; bottom:-10px; left:50px; filter: invert(0.05)"/>

</div v-click> 


<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />

---
layout: two-cols-header
---

## **Methods** -- Modelling approach


::left::

- Modelling domain $\rightarrow$ 2D materials (for now)
- Load-controlled uniaxial tension with multi-point constraints
- Timoshenko beam elements $(\bar{\rho} < 20 \%):$

<img src="/media/figures/beamElement.png" style="position:relative; width:300px; bottom:-20px; right:-50px; filter: invert(100%)">

<hr style="height:90pt; visibility:hidden;" />

::right::

<img src="/media/figures/bcs.png" style="position:fixed; width:425px; bottom:50px; right:50px">


<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />

---
layout: two-cols-header
---

## **Methods** -- Fracture toughness maximization

<p> </p>

::left::

- Optimization problem (1 crack configuration):
$$
\begin{align*}
\max_{\mathbf{x}=\{x_w, \mathbf{x}_{\text{uc}}\}} \quad & \lambda(\mathbf{x}) = \frac{\sigma_c}{\sigma_{\max}(\mathbf{x})} && \text{Load scaling factor}\\[2pt]
\text{s.t.}       \quad & \mathbf{K}(\mathbf{x}) \mathbf{u}(\mathbf{x}) = \mathbf{f}, && \text{Static equilibrium} \\[2pt]
                  \quad & g_{\text{iso}}(\mathbf{C}^H(\mathbf{x})) \leq 0, && \text{Isotropic unit cell} \\[2pt]
                  \quad & g_{E}(\mathbf{C}^H(\mathbf{x})) \leq 0, && 
                  \text{Unit cell stiffness} \\[2pt]
                  \quad & \frac{V(\mathbf{x})}{V_0 \, f_V} - 1 \leq 0, && \text{Volume constraint}  \\[2pt]
                  \quad & \mathbf{0} \leq \mathbf{x}  \leq  \mathbf{1}
\end{align*}
$$


<div v-click> 

$$g_{E}(\mathbf{C}^H(\mathbf{x})) = 1 - \frac{E^H(\mathbf{x})}{E_{\text{HS}} \, f_E}$$  

$$\begin{align*}
&E_{\text{HS}} = \frac{1}{3}E_s w \bar{\rho}_{uc} && \text{HS-bound beam structrure} \\
&f_E  && \text{Young's modulus fraction}
\end{align*}$$

</div v-click> 


::right::


<div v-click> 

<img src="/media/figures/interpolation.svg" style="position:relative; width:600px; bottom:0px; right:-20px; filter: invert(.05)"/>

</div v-click> 

 <!-- $$\max_{\mathbf{x}}   \quad \mathcal{J}(\mathbf{x})=\lambda(\mathbf{x}) - c_{G_x} \lambda^{(0)} M_{\text{nd}}(\mathbf{x}) $$ -->

<br>

<div v-click> 

- Penalize with $M_{\text{nd}}$ to obtain black-white:
$$ \max_{\mathbf{x}\in \mathbb{R}^{N_e^\text{uc}}} \quad \mathcal{J}(\mathbf{x})=\lambda(\mathbf{x}) - c_{G_x} \lambda^{(0)} M_{\text{nd}}(\mathbf{x})  $$

</div v-click> 

<div v-click> 

- Maximize the worst case using $p$-norm: 

$$\max_{\mathbf{x}} \quad \min(\mathcal{J}_k) \approx  \mathcal{J}_{\text{PN}}, \qquad k = 1,\dots,N_c$$

</div v-click> 

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />

---

## **Results** -- optimization, $\footnotesize x_{w0} = 0.75$

<p> </p>

<!-- 

<v-click> 
<img src="/media/plots/structure_comp_1.png" style="position:fixed; width:500px; bottom:20px; right:50px"/>
</v-click> -->


<div v-click.hide at="0">

<p style="position: fixed; top: 80px; left: 60px"> - Worst case optimization </p> 

<img src="/media/results/multi_reference_optimized_xw0_0.75_epsilonHom_0.025.svg" style="position:fixed; width:65%; bottom:10px; left:200px; filter: invert(.05)"/>

</div>

<div v-after>

<p style="position: fixed; top: 80px; left: 60px"> - Worst case benchmark</p> 

<img src="/media/results/multi_reference_benchmark_xw0_0.75_epsilonHom_0.025.svg" style="position:fixed; width:65%; bottom:10px; left:200px; filter: invert(.05)"/>

</div>


<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />

---
layout: two-cols-header
dragPos:
  square1: 189,164,90,67
  square2: 354,266,90,67
---

## **Results** -- Reference structures


::left::

<img src="/media/results/fig5_reference_plot.svg" style="position:relative; width:100%; top:-80px; left:50px; filter: invert(.05)"/>

<div v-click>

<v-drag-arrow width=1; pos="358,298,-57,27"/>
<v-drag-arrow width=1; pos="237,227,56,33"/>

<img v-drag="'square1'" src="/media/results/triangular_2x2.svg" class="addBorder">

<img v-drag="'square2'" src="/media/results/kagome_2x2.svg" class="addBorder">

</div>

::right::

<div v-click>


<img src="/media/results/fig6_unitCellMeshSensitivityStudy.svg" style="position:relative; width:90%; top:-80px; left:80px; filter: invert(.05)"/>

</div>


<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />

---

## **Results** -- optimization, $\footnotesize x_{w0} = 0.25$

<p> </p>

<!-- 

<v-click> 
<img src="/media/plots/structure_comp_1.png" style="position:fixed; width:500px; bottom:20px; right:50px"/>
</v-click> -->


<div v-click.hide at="0">

<p style="position: fixed; top: 80px; left: 60px"> - Worst case optimization </p> 

<img src="/media/results/multi_reference_optimized_xw0_0.75_epsilonHom_0.025.svg" style="position:fixed; width:65%; bottom:10px; left:200px; filter: invert(.05)"/>

</div>

<div v-after>

<p style="position: fixed; top: 80px; left: 60px"> - Worst case benchmark</p> 

<img src="/media/results/multi_reference_benchmark_xw0_0.75_epsilonHom_0.025.svg" style="position:fixed; width:65%; bottom:10px; left:200px; filter: invert(.05)"/>

</div>


<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />