## **Architected lattice materials** -- Applications
<p> </p>



- High performance low density materials 
- Enabled by additive manufacturing using both metals and polymers

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
    <img src="/media/litterature/Ashby_E.png" style="width:100%; filter:invert(0.03)"/>
    <p style="position:relative; top:-35px; right:10px; text-align:right"> <sup>1)</sup> </p>  
  </div>
  
  <div>
    Tailor, and improve fracture toughness?
    <img src="/media/ashby/image1-3.png" style="width:357px; filter:invert(0.03) "/>
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


<!--
<v-click>

 - Asymptotic $K$-displacement field for Mode I: 
$$
\textcolor{green}{
u_1 = \frac{K_\text{I}}{2\sqrt{2\pi}G} r^{1/2} \left[(\kappa - \cos\theta)\cos\frac{\theta}{2}\right] }
$$ 
$$
\textcolor{green}{
u_2 = \frac{K_\text{I}}{2\sqrt{2\pi}G} r^{1/2} \left[(\kappa - \cos\theta)\sin\frac{\theta}{2}\right] }
$$


$$ \kappa = 
</v-click> -->

<style>
.boxed-equation {
  border: 2px solid #e47323; 
  padding: 5px; 
  border-radius: 5px; 
  display: inline-block; 
  margin: 10px 0;
}
.transparent-box {
  background: rgba(255, 255, 255, 0.5);
  border-radius: 5px;
  padding: 0px;
  width: 430px;
  height: 240px;
}
</style>

## **Background** -- Fracture toughness in lattice materials

::left::


<div v-click>

####  **Fracture toughness: $K_c$**
-  Critical value the stress intensity factor $K$


- For crack in an infinitely wide plate subjected to a remote tensile stress:
 $$K_{\text{I}} = \sigma \sqrt{\pi a}$$

- LEFM: $\quad K_{\text{I}} = K_{\text{Ic}} \quad$ gives $\quad \sigma_\text{c} = K_{\text{Ic}}/\sqrt{\pi a}$

</div>

<div v-click='2'>

<div style="position:fixed; top:75px; left:50px;background: rgba(255, 255, 255, 0.5);" class="transparent-box"> </div>

- When applying the $K_{\text{I}}$-displacement field we find the mode I fracture toughness as:

$$ K_{\text{Ic}} = K_{\text{I}} \lambda $$

- Where <div class="boxed-equation"> $\lambda = \dfrac{\sigma_\text{f}}{\sigma_{\max}}$ </div> is the load scaling factor

</div>


<div style="height: 0px;"></div>

::right::

<div v-click='0'>
<img src="/media/litterature/infinite.svg" style="position:fixed; width:310px; bottom:50px; right:100px; filter: invert(.05)"/>

</div v-click>


<div v-click='2'>

<img src="/media/figures/Kfield_01.svg" style="position:fixed; width:475px; bottom:50px; right:10px; filter: invert(.05)"/>

</div v-click>

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />


---
layout: two-cols-header
dragPos:
  square1: 275,251,73,54
  square2: 147,84,146,108
---

<style>
.boxed-equation2 {
  border: 2px solid #e47323; 
  padding: 5px; 
  border-radius: 5px; 
  display: inline-block;
  margin: 10px 0;
}
</style>



## **Background** -- State of the art

#### $\hspace{40mm}$ <div class="boxed-equation2"> $K_{\text{Ic}} = D \bar{\rho}^d  \sigma_{\text{f}} \sqrt{l}$ </div>

::left::

<div v-click.hide>

<img src="/media/litterature/fleckRhoKIC.png" style="position:relative; width:100%; top:10px; left:100px; filter: invert(.05)"/>

<v-drag-arrow width=1 color=rgb(240,160,90) pos="341,269,62,-54"/>
<v-drag-arrow width=1 color=rgb(240,160,90) pos="289,182,45,20"/>

<img v-drag="'square1'" src="/media/results/triangular_2x2.svg" class="addBorder">
<img v-drag="'square2'" src="/media/results/kagome_2x2.svg" class="addBorder">

<p style="position:fixed; top:410px; left:550px; font-weight: bold"> <sup>1)</sup> </p>

</div>

<div v-click="1">

<img src="/media/litterature/demiregularResultsFull.png" style="position:fixed; width:60%; top:200px; left:5px; filter: invert(.05)"/>
<p style="position:fixed; bottom:70px; left:550px; font-weight: bold"> <sup>2)</sup> </p>

</div>

::right::

<div v-click="'1'">

<img src="/media/litterature/demiregularStructures.png" style="position:relative; width:85%; top:-100px; left:110px; filter: invert(.05)"/>
<p style="position:fixed; bottom:10px; right: 20px; font-weight: bold"> <sup>2)</sup> </p>

</div>

<Footnotes>
  <Footnote :number=1> Fleck and Qiu (2007) </Footnote>
  
  <div v-click="1">
  <Footnote :number=2> Omidi and St-Pierre (2023) </Footnote>
  </div v-click>

</Footnotes> 

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />

---
layout: two-cols-header
---

## **Analysis** -- Normalizing with $\sqrt{l}$ or $\sqrt{L}$


- Results shown for $\bar{\rho}$ = 15 %

<img src="/media/results/pseudo_kagome.png" style="position:relative; width:60%; top:10px; left:50px; filter: invert(.05)"/>

<!-- <img src="/media/figures/structures.svg" style="position:fixed; width:20%; top:90px; right:90px; filter: invert(.05)"/> -->

<v-click>


<style>
.centered-up {
  display: block;
  margin-left: auto;
  margin-right: auto;
  position: relative;
  left: -90px;
  top: 30px;
}
</style>

<div
  v-motion
  :click-1="{ x: 190, y:63 }"
  :click-2="{ x: 190, y:86 }"
>
  <img v-drag="[0,0,310,25,0]" class="addBorder">
</div>


<div>
  <img src="/media/results/pseudo_kagome_table.svg" class="centered-up" style="width:300px; filter: invert(0.10)"/>
</div>

<figure style="position:fixed; top: 175px; right:0px; display: table; filter:invert(0.90)" >
  <SlidevVideo muted autoreset autoplay loop style="position:relative; top:0px; left:0px; width:350px">
    <source src="/media/animations/pseudo_kagome.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 


</v-click>

<v-click> 

$\textcolor{white}{ }$

</v-click>


<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />


---
layout: two-cols-header
---

## **Results** -- Normalizing with $\sqrt{l}$ or $\sqrt{L}$

<p> </p>


<div
  v-motion
  :enter="{ x: 520, y: 0 }"
  :click-1="{ x: 700, y: 0 }"
>
  <img v-drag="[0,0,180,310,0]" class="addBorder">
</div>


<div
  v-motion
  :enter="{ x: 515, y:325 }"
  :click-1="{ x: 625, y:325 }"
>
  <img v-drag="[0,0,110,97,0]" class="addBorder">
</div>


<img src="/media/results/pseudo_kagome_all.png" style="position:relative; width:100%; top:10px; left:0px; filter: invert(.05)"/>


<style>
.centered-up {
  display: block;
  margin-left: auto;
  margin-right: auto;
  position: relative;

  top: 30px;
}
</style>

<div>
  <img src="/media/results/pseudo_kagome_table_all.svg" class="centered-up" style="width:600px; filter: invert(0.10)"/>
</div>

<v-click> 

$\textcolor{white}{ }$

</v-click>


<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />


---
layout: two-cols-header
---

## **Results** -- Comparison of structures

<p> </p>

::left:: 

- #### **Scaling laws**:

$$ E = B \bar{\rho}^b E_s  $$
$$ K_{\text{Ic}} = M \bar{\rho}^d \sigma_\text{f} \sqrt{L}  $$

- Critical energy release rate: $G_{\text{c}} = (1 - \nu^2) \dfrac{K_{\text{Ic}}^2}{E}$

$$ \frac{G_\text{c} E_ \text{s}}{\sigma_\text{f}^2 L} = (1 - \nu^2) \frac{M^2}{B} \bar{\rho}^{2d-b}   $$

<img src="/media/results/comparison_table.svg" style="position:relative; width:90%; top:0px; left:40px; filter: invert(.05)"/>

::right::

<img src="/media/results/K_Ic_plot_all.svg" style="position:relative; width:75%; top:-30px; left:80px; filter: invert(.05)"/>

<img src="/media/results/G_c_plot_all.svg" style="position:relative; width:75%; top:-25px; left:80px; filter: invert(.05)"/>

<v-click>


</v-click>

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />



---
layout: two-cols-header
---

## **Methods** -- Fracture toughness maximization

<p> </p>

::left::


$${1|1,2|3|4|5|all}
\begin{aligned}
\max_{\mathbf{x}=\{x_t, \mathbf{x}_{\text{uc}}\}} \quad & \mathcal{J}= \lambda(\mathbf{x},\mathbf{u}(\mathbf{x})) - c \, M_{\text{nd}}(\mathbf{x}) && \\[2pt] % && \text{Load scaling factor}\\[2pt]
\text{s.t.}       \quad & \mathbf{K}(\mathbf{x}) \mathbf{u}(\mathbf{x}) = \mathbf{f}, && \text{Static equilibrium} \\[2pt]
                  \quad & g_{\text{vol}} = \bar{\rho}(\mathbf{x})/\bar{\rho}^* - 1 \leq 0, && \text{Ressource constraint}  \\[2pt]
                  \quad & g_{\text{iso}}(\mathbf{C}(\mathbf{x})) \leq 0, && \text{Isotropic unit cell} \\[2pt]
                  \quad & g_{E} = 1 -\frac{E(\mathbf{x})}{E_{\text{HS}}f_E} \leq 0, && 
                  \text{Unit cell stiffness} \\[2pt]

                  \quad & \mathbf{0} \leq \mathbf{x}  \leq  \mathbf{1}
\end{aligned}
$$

- Load scaling factor: $\quad \lambda(\mathbf{x},\mathbf{u}(\mathbf{x})) = \dfrac{\sigma_\text{f}}{\sigma_{\max}(\mathbf{x},\mathbf{u}(\mathbf{x}))}$

- Global beam thickness: $\quad t(x_t) = t_{\min} + x_t(t_{\max} - t_{\min})$

- Measure of non-discreteness: $M_{\text{nd}}(\mathbf{x}) = \frac{4}{N_e} \sum_{e=1}^{N_e} x_e(1-x_e)$


::right::

<img src="/media/figures/homogenization_new.svg" style="position:fixed; width:350px; top:80px; right:0px; filter: invert(0)"/>
<img src="/media/figures/Kfield_optimization.svg" style="position:fixed; width:175px; bottom:10px; right:100px; filter: invert(0.02)"/>

 <!-- $$\max_{\mathbf{x}}   \quad \mathcal{J}(\mathbf{x})=\lambda(\mathbf{x}) - c_{G_x} \lambda^{(0)} M_{\text{nd}}(\mathbf{x}) $$ -->

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />


---
layout: two-cols-header
---
## **Results** -- Fracture toughness maximization

<p> </p> 

<style>
.transparent-box {
  background: rgba(255, 255, 255, 0.5);
  border-radius: 5px;
  padding: 0px;
  width: 360px;
  height: 335px;
}
</style>

- Results shown for a 10% **triangular** initial guess with $\bar{\rho}^* = 15 \%$, $N_{\text{bc}}=4$, $f_\text{E}=0.5$

<img src="/media/results/res_none_fE_0.5_01.png" style="position:fixed; width:350px; top:130px; left:60px; filter: invert(0.025)"/>

<div v-click='+2'>


<div style="position:fixed; top:125px; left:55px; background: rgba(240, 240, 240, 0.5);" class="transparent-box">  </div>


<img src="/media/results/res_kagome-indices-Nbc-4-htype--2_fE_0.5_01.png" style="position:fixed; width:350px; top:130px; left:420px; filter: invert(0.025)"/>


<p style="position:fixed; width:200px; bottom:125px; right:-20px; font-size:10pt"> <b> Triangular </b> initial guess exaggerated <b> 5x </b> </p>

<img src="/media/results/initialGuess_x5.png" style="position:fixed; width:180px; bottom:10px; right:10px; filter: invert(0.025)"/>

</div>

<div
  v-motion
  :enter="{ x: 0, y:25 }"
  :click-1="{ x: 178, y:25 }"
  :click-2="{ x: 360, y:25 }"
  :click-3="{ x: 538, y:25 }"
>
  <img v-drag="[0,0,180,310,0]" class="addBorder">
</div>

<div style="height: 330px;"></div>

- Best performing (triangular) structure:   <div class="boxed-equation2">$\lambda_{\max}=208$</div>
- Note, the triangular and Kagome structures satisfies $\bar{\rho} = 15 \%$ for $t=0.548$ mm

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />

<v-clicks> 

- $\textcolor{white}{ }$
- $\textcolor{white}{ }$
- $\textcolor{white}{ }$

</v-clicks>

---
layout: two-cols-header
---
## **Results** -- Fracture toughness maximization

<p> </p> 



- Results shown for a 10% **triangular** initial guess with $\bar{\rho}^* = 15 \%$, $N_{\text{bc}}=4$, $f_\text{E}=0.01$

<img src="/media/results/res_kagome-indices-Nbc-4-htype--2_fE_0.01_01.png" style="position:relative; width:475px; top:0px; left:200px; filter: invert(0.025)"/>


<v-click>

- Results shown for a 10% **Kagome** initial guess with $\bar{\rho}^* = 15 \%$, $N_{\text{bc}}=4$, $f_\text{E}=0.10$

<img src="/media/results/res_kagome-indices-Nbc-4-htype-0_fE_0.1_01.png" style="position:relative; width:475px; top:0px; left:200px; filter: invert(0.025)"/>

</v-click>

<div style="height: 0px;"></div>


<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" />



<!-- 


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

<img style="position:fixed; top:10px; right:50px; width:200px;" src="/media/DTU/Villum_black.png" v-bind="props" /> -->
