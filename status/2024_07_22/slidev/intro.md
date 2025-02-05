---
layout: two-cols-header
---

## Load control with multipoint constraints

::left::

<figure style="position:relative; top:0px; left:0px; display: table" >
  <figcaption> <p style="font-size: normal; 
                         font-weight: normal;
                         text-align: center"> No MPC </p> 
  <img src="/media/mpc_test/mpc_test_no_mpc.png" style="width:350px">
  </figcaption>
</figure> 

::right::

<figure style="position:relative; top:40px; left:0px; display: table" >
  <figcaption> <p style="font-size: normal; 
                         font-weight: normal;
                         text-align: center;"> With MPC </p> 
  <img src="/media/mpc_test/mpc_test_with_mpc.png" style="width:350px">
  </figcaption>
</figure> 

<img src="/media/mpc_test/mpc_test_bc.png" 
     style="position:fixed; top:10px; right:40px; width:150px"/>


<!-- 

add notes here

-->

---
layout: two-cols-header
zoom: 0.9
---

### Fracture energy optimization - load control

::left::

$$
\footnotesize
\begin{align*}
\max_{\mathbf{x}} \quad & W_f = \frac{1}{2} P_0 \lambda^2 U  \\
\text{s.t.}       \quad & \mathbf{K} \mathbf{u} = \mathbf{f}, \\
                  \quad & g_{iso}(\mathbf{C}^H_{uc}) \leq 0, \\
                  \quad & g_{stiff}(\mathbf{C}^H_{uc}) \leq 0, \\
                  \quad & \frac{V}{V_0 V^\ast} - 1 \leq 0, \\
                  \quad & \mathbf{0} \leq \mathbf{x} \leq \mathbf{1}
\end{align*}
$$
with
$$
\footnotesize
\begin{align*}
g_{stiff}(\mathbf{C}_{uc}^H) &= 1 - \frac{C_{11}^H + C_{22}^H}{2C_0} \\ 
C_0 &= C^\ast (C_{11}^H)_{tri}  =  C^\ast \frac{3Ew}{8}\bar{\rho}_{uc}
\end{align*}
$$

<!-- 
$$
\footnotesize
\begin{align*}
t_e(x_e) &= t_{\min} + x_e^{q_t}(t_{\max} - t_{\min}) \\
\tilde{\sigma}_e &= x_e^{q_\sigma} \sigma_e %\\ 
% q_\sigma^{(i+1)} &= q_{\sigma}^{(i)} + q_\sigma^+ \text{ every 50th iteration}
\end{align*}
$$ -->

Ran all combinations of

$$
\footnotesize
\begin{align*}
 p &= \{4, 8, 12 \}, \ &&N_{uc} = \{2, 3, 4 \}, \\
 C^\ast&=\{0.4, 0.5, 0.6\}, &&q_t =\{1.5, 2\}
\end{align*}
$$

::right::

<img src="/media/parameter_study/q_sig.png" 
     style="position:relative; top:10px; left:100px; width:300px"/>

$$\footnotesize{N_{uc}=3}$$

<img src="/media/unit_cell_3x3.png" 
     style="position:relative; top:-20px; left:100px; width:300px"/>


---
layout: two-cols-header
zoom: 0.9
---

### Fracture energy optimization - load control

$\footnotesize \ \ V^\ast = 0.25, \ p = 8, \ N_{uc} = 2$

Intermediate stiffness fraction: $C^\ast = 0.60$

::left::

<figure style="position:relative; top: 20px; left:0px; display: table" >
  <SlidevVideo muted autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:600px">
    <source src="/media/parameter_study/Cfrac_0.6/UnitCell_le_0.062_vfrac_0.25_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 


:: right :: 

<figure style="position:relative; top: 20px; left:0px; display: table" >
  <SlidevVideo muted autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:600px">
    <source src="/media/parameter_study/Cfrac_0.6/UnitCell_le_0.062_vfrac_0.25_cmp_stress.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 

<img src="/media/parameter_study/Cfrac_0.6/UnitCellGrid_designHistory_00099.jpeg" 
     style="position:fixed; top:10px; right:100px; width:400px"/>

---
layout: two-cols-header
zoom: 0.9
---

### Fracture energy optimization - load control

$\footnotesize \ \ V^\ast = 0.25, \ p = 8, \ N_{uc} = 2$

High stiffness fraction: $C^\ast = 0.95$

::left::

<figure style="position:relative; top: 20px; left:0px; display: table" >
  <SlidevVideo muted autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:600px">
    <source src="/media/parameter_study/Cfrac_0.95/UnitCell_le_0.062_vfrac_0.25_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 


:: right :: 

<figure style="position:relative; top: 20px; left:0px; display: table" >
  <SlidevVideo muted autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:600px">
    <source src="/media/parameter_study/Cfrac_0.95/UnitCell_le_0.062_vfrac_0.25_cmp_stress.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 

<img src="/media/parameter_study/Cfrac_0.95/UnitCellGrid_designHistory_00099.jpeg" 
     style="position:fixed; top:10px; right:100px; width:400px"/>


---

##### $\footnotesize \ \ V^\ast = 0.25, \  p = 8, \ q_{t} = 1.5$

<figure style="position:fixed; top:85px; left:40px; display: table" >
  <SlidevVideo muted v-click=1 autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:325px">
    <source src="/media/parameter_study/Cfrac_nuc/UnitCell_le_0.062_vfrac_0.25_p_8_Cfrac_0.40_nuc_2_qt_1.50_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 

<figure style="position:fixed; top:300px; left:40px; display: table" >
  <SlidevVideo muted v-click=1 autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:325px">
    <source src="/media/parameter_study/Cfrac_nuc/UnitCell_le_0.062_vfrac_0.25_p_8_Cfrac_0.40_nuc_3_qt_1.50_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 


<figure style="position:fixed; top:85px; left:315px; display: table" >
  <SlidevVideo muted v-click=2 autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:325px">
    <source src="/media/parameter_study/Cfrac_nuc/UnitCell_le_0.062_vfrac_0.25_p_8_Cfrac_0.50_nuc_2_qt_1.50_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 

<figure style="position:fixed; top:300px; left:315px; display: table" >
  <SlidevVideo muted v-click=2 autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:325px">
    <source src="/media/parameter_study/Cfrac_nuc/UnitCell_le_0.062_vfrac_0.25_p_8_Cfrac_0.50_nuc_3_qt_1.50_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 


<figure style="position:fixed; top:85px; left:585px; display: table" >
  <SlidevVideo muted v-click=3 autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:325px">
    <source src="/media/parameter_study/Cfrac_nuc/UnitCell_le_0.062_vfrac_0.25_p_8_Cfrac_0.60_nuc_2_qt_1.50_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 

<figure style="position:fixed; top:300px; left:585px; display: table" >
  <SlidevVideo muted v-click=3 autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:325px">
    <source src="/media/parameter_study/Cfrac_nuc/UnitCell_le_0.062_vfrac_0.25_p_8_Cfrac_0.60_nuc_3_qt_1.50_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 



<p style="position:fixed; top:50px; left:150px" font-size="16px">  C* = 0.4 </p>
<p style="position:fixed; top:50px; left:430px" font-size="16px">  C* = 0.5 </p>
<p style="position:fixed; top:50px; left:700px" font-size="16px">  C* = 0.6 </p>
<p style="position:fixed; top:170px; left:5px" font-size="16px" rotate="-90deg" >  Nuc = 2  </p>
<p style="position:fixed; top:380px; left:5px" font-size="16px" rotate="-90deg" >  Nuc = 3  </p>

---

##### $\footnotesize \ \ V^\ast = 0.25, \  p = 8, \ q_{t} = 2.0$

<figure style="position:fixed; top:85px; left:40px; display: table" >
  <SlidevVideo muted v-click=1 autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:325px">
    <source src="/media/parameter_study/Cfrac_nuc/UnitCell_le_0.062_vfrac_0.25_p_8_Cfrac_0.40_nuc_2_qt_2.00_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 

<figure style="position:fixed; top:300px; left:40px; display: table" >
  <SlidevVideo muted v-click=1 autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:325px">
    <source src="/media/parameter_study/Cfrac_nuc/UnitCell_le_0.062_vfrac_0.25_p_8_Cfrac_0.40_nuc_3_qt_2.00_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 


<figure style="position:fixed; top:85px; left:315px; display: table" >
  <SlidevVideo muted v-click=2 autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:325px">
    <source src="/media/parameter_study/Cfrac_nuc/UnitCell_le_0.062_vfrac_0.25_p_8_Cfrac_0.50_nuc_2_qt_2.00_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 

<figure style="position:fixed; top:300px; left:315px; display: table" >
  <SlidevVideo muted v-click=2 autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:325px">
    <source src="/media/parameter_study/Cfrac_nuc/UnitCell_le_0.062_vfrac_0.25_p_8_Cfrac_0.50_nuc_3_qt_2.00_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 


<figure style="position:fixed; top:85px; left:585px; display: table" >
  <SlidevVideo muted v-click=3 autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:325px">
    <source src="/media/parameter_study/Cfrac_nuc/UnitCell_le_0.062_vfrac_0.25_p_8_Cfrac_0.60_nuc_2_qt_2.00_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 

<figure style="position:fixed; top:300px; left:585px; display: table" >
  <SlidevVideo muted v-click=3 autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:325px">
    <source src="/media/parameter_study/Cfrac_nuc/UnitCell_le_0.062_vfrac_0.25_p_8_Cfrac_0.60_nuc_3_qt_2.00_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 



<p style="position:fixed; top:50px; left:150px" font-size="16px">  C* = 0.4 </p>
<p style="position:fixed; top:50px; left:430px" font-size="16px">  C* = 0.5 </p>
<p style="position:fixed; top:50px; left:700px" font-size="16px">  C* = 0.6 </p>
<p style="position:fixed; top:170px; left:5px" font-size="16px" rotate="-90deg" >  Nuc = 2  </p>
<p style="position:fixed; top:380px; left:5px" font-size="16px" rotate="-90deg" >  Nuc = 3  </p>



