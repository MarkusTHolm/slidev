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
  <Footnote :number=1> Jenett et al. (2017) </Footnote>
  <Footnote :number=2> Inspired by Tankasala et al. (2015) </Footnote>
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

- Fracture toughness $:=$ Critical value of the Mode I stress intensity factor

<v-clicks>

- Mode I stress-intensity factor for an infinite plate: 
$$K_{\text{I}} = \sigma_0 \sqrt{\pi a}$$

- So, $K_\text{I} = O(\sigma_0 \sqrt{a})$ and we define

$$ K_{\text{Ic}} = \sigma_c \sqrt{a} = \lambda \sigma_0 \sqrt{a} $$

- Where <div class="boxed-equation"> $\lambda = \dfrac{\sigma_f}{\sigma_{\max}}$ </div> is the load scaling factor

</v-clicks>

::right::

<div v-click.hide>

<img src="/media/figures/fracture_toughness_1.svg" style="position:fixed; width:425px; bottom:50px; right:25px"/>

</div>

<div v-after>

<img src="/media/figures/fracture_toughness_2.svg" style="position:fixed; width:425px; bottom:50px; right:25px"/>

</div>

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
  
---
layout: two-cols-header
---

## **Results** -- Without normalization

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
  <img src="/media/results/lamMax.png" class="centered-up" style="width:475px; filter: invert(0.10)"/>
</div>

</v-click>
  

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

- The problem when optimizing:
<div>
  <img src="/media/figures/unitCell_Nbc234.svg" class="centered-up" style="width:750px; filter: invert(0.0)"/>
</div>

<p> </p>

<v-click>

- **Future work**:
  - Attempting optimization on fine meshes
  - Relaxing isotropy
  - ... suggestions?
</v-click>