## **Architected lattice materials** -- Applications
<p> </p>



- Enabled by additive manufacturing
- Metals and polymers

- <span v-mark.orange.v-mark="1"> Aerospace, </span> <span v-mark.orange.v-mark="2"> orthopedic implants, </span> <span v-mark.orange.v-mark="3"> sporting gear </span>, etc.


<div v-click="4">

- Active research field

</div v-click>

<img src="/media/MetalAm/ssm-slm-inconel-sparrow.png" style="position:fixed; bottom:80px; left:-40px; width:325px"/>
<p style="position:fixed; bottom:50px; left:40px; text-align:left; font-weight: lighter"> <sup>1)</sup> </p> 


<img src="/media/MetalAm/ESAbracket.png" style="position:fixed; bottom:90px; right:350px; width:375px"/>
<p style="position:fixed; bottom:100px; right:615px; text-align:left; font-weight: lighter"> <sup>2)</sup> </p>  
 

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

## **Architected lattice materials** -- Properties
<p> </p>
  

<div class="grid grid-cols-2 gap-4">
  <div>
    Tailor stiffness 
    <img src="/media/ashby/g23.png" style="width:600px; filter:invert(0.05)"/>
    <p style="position:relative; top:-35px; right:10px; text-align:right"> <sup>1)</sup> </p>  
  </div>
  
  <div>
    Tailor, and improve fracture toughness?
    <img src="/media/ashby/image1-3.png" style="width:390px; filter:invert(0.03) "/>
    <p style="position:relative; top:-35px; right:50px; text-align:right"> <sup>2)</sup> </p>  
  </div>

</div>

<Footnotes separator>
  <Footnote :number=1> Inspired by Jenett et al. (2017) </Footnote>
  <Footnote :number=2> Tankasala, Deshpande and Fleck (2015) </Footnote>
</Footnotes> 

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />

---
layout: two-cols-header
---

<style>
.boxed-equation {
  border: 2px solid #e47323; 
  padding: 5px; 
  border-radius: 5px; 
  display: inline-block; 
  margin: 10px 0;
}
</style>

## **Analysis** -- Fracture toughness in lattice materials

::left::

- Fracture toughness $:=$ Critical value of the stress intensity factor (SIF)

<v-clicks>

- Mode I SIF for an infinite homogenous (solid) plate: 
$$K_{\text{I}} = \sigma_0 \sqrt{\pi a}$$

- So, $K_\text{I} = O(\sigma_0 \sqrt{a})$ and we define

$$ K_{\text{Ic}} = \sigma_c \sqrt{a} = \lambda \sigma_0 \sqrt{a} $$

- Where <div class="boxed-equation"> $\lambda = \dfrac{\sigma_f}{\sigma_{\max}}$ </div> is the load scaling factor

</v-clicks>

::right::

<div v-click.hide>

<img src="/media/figures/Kfield_01.svg" style="position:fixed; width:425px; bottom:50px; right:25px"/>

</div>

<div v-after>

<img src="/media/figures/Kfield_02.svg" style="position:fixed; width:425px; bottom:50px; right:25px"/>

</div>

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />


---
layout: two-cols-header
dragPos:
  square1: 373,151,73,54
  square2: 226,158,73,53
---

## **Results** -- State of the art

::left::

<v-click>

<img src="/media/litterature/fleckRhoKIC.png" style="position:relative; width:75%; top:10px; left:100px; filter: invert(.05)"/>

<v-drag-arrow width=1 color=rgb(240,160,90) pos="379,174,-34,-31"/>
<v-drag-arrow width=1 color=rgb(240,160,90) pos="267,163,45,-30"/>

<img v-drag="'square1'" src="/media/results/triangular_2x2.svg" class="addBorder">
<img v-drag="'square2'" src="/media/results/kagome_2x2.svg" class="addBorder">

<p style="position:fixed; top:285px; left:455px; font-weight: lighter"> <sup>1)</sup> </p>

</v-click>

<v-click>

<img src="/media/litterature/demiregularResultsFull.png" style="position:relative; width:100%; top:20px; left:50px; filter: invert(.05)"/>
<p style="position:fixed; bottom:5px; left:510px; font-weight: lighter"> <sup>2)</sup> </p>

</v-click>

::right::

<v-click at="+0">

<img src="/media/litterature/demiregularStructures.png" style="position:relative; width:75%; top:10px; left:80px; filter: invert(.05)"/>
<p style="position:fixed; bottom:10px; right:100px; font-weight: lighter"> <sup>2)</sup> </p>

</v-click>

<Footnotes>
  <div v-click="1">
  <Footnote :number=1> Fleck and Qiu (2007) </Footnote>
  </div v-click>
  
  <div v-click="2">
  <Footnote :number=2> Omidi and St-Pierre (2023) </Footnote>
  </div v-click>

</Footnotes> 

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />


---
layout: two-cols-header
---

## **Results** -- Normalizing with $\sqrt{l}$

<p> </p>

<div class="grid grid-cols-2 gap-4">

  <v-click>

  <div>  
    <img src="/media/results/resNorm_tri.svg" style="width:325px; margin: auto"/>
  </div>
  
  <div>
    <img src="/media/results/resNorm_kag.svg" style="width:325px; margin: auto"/>
  </div>

  <div style="position:fixed; right:30px; top:135px">
    <img src="/media/results/colorBarsig_0_15.svg" style="width:50px"/>
  </div>

  </v-click>

  <v-clicks>

  <div>
    <img src="/media/results/resNorm_kagII.svg" style="width:325px; margin: auto"/>
  </div>

  <div>
    <img src="/media/results/resNorm_kagIIopt.svg" style="width:325px; margin: auto;"/>
  </div>  

  </v-clicks> 

</div>

<v-click>

$$ \footnotesize \textbf{Table 1: } \lambda_{\max}/\sqrt{l} $$


<style>
.centered-up {
  display: block;
  margin-left: auto;
  margin-right: auto;
  position: relative;
  top: -20px;
}
</style>

<div>
  <img src="/media/results/lamMaxNorm.png" class="centered-up" style="width:300px; filter: invert(0.10)"/>
</div>

</v-click>

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />


---
layout: two-cols-header
---

## **Results** -- Without normalization ($\footnotesize W/L=24$)

<p> </p>

<div class="grid grid-cols-2 gap-4">

  <div>  
    <img src="/media/results/res_tri.svg" style="width:325px; margin: auto"/>
  </div>
  
  <div style="position:fixed; right:30px; top:135px">
    <img src="/media/results/colorBarsig_0_15.svg" style="width:50px"/>
  </div>

  <v-clicks>

  <div>
    <img src="/media/results/res_kag-1.svg" style="width:325px; margin: auto"/>
  </div>

  <div>
    <img src="/media/results/res_kag.svg" style="width:325px; margin: auto"/>
  </div>

  <div>
    <img src="/media/results/res_kag+1.svg" style="width:325px; margin: auto;"/>
  </div>  

  </v-clicks> 

</div>

<v-click>

$$ \footnotesize \textbf{Table 2: } \lambda_{\max} $$


<style>
.centered-up {
  display: block;
  margin-left: auto;
  margin-right: auto;
  position: relative;
  top: -20px;
}
</style>

<div>
  <img src="/media/results/lamMax.png" class="centered-up" style="width:450px; filter: invert(0.10)"/>
</div>

</v-click>

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />


---


<style>
.centered-up {
  display: block;
  margin-left: auto;
  margin-right: auto;
  position: relative;
  top: 0px;
}
</style>

# **Conclusions**

- Fracture toughness should be normalized with unit cell size, $L$, instead of beam length, $l$
- The problem when optimizing: $a/l$ vs. $a/L$
<div>
  <img src="/media/figures/unitCell_Nbc234.svg" class="centered-up" style="width:650px; filter: invert(0.0)"/>
</div>

<p> </p>

<v-click>

### **Future work**
  - Optimization for fixed $a/L$ with different $W/L$
  - Relaxing isotropy
</v-click>

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />


---
layout: two-cols-header
---
## **Methods** -- Fracture toughness maximization

<p> </p>

::left::

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
$$ \max_{\mathbf{x}=\{x_w, \mathbf{x}_{\text{uc}}\}} \quad \mathcal{J}(\mathbf{x})=\lambda(\mathbf{x}) - c_{M_{nd}} \lambda^{(0)} M_{\text{nd}}(\mathbf{x})  $$

</div v-click> 


<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />

---