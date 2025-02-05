---
layout: two-cols-header
zoom: .75
---

## Fracture energy optimization - load control

::left::

$$
\begin{align*}
\max_{\mathbf{x}} \quad & W_f = \frac{1}{2} P_0 \lambda^2 U  \\
\text{s.t.}       \quad & \mathbf{K} \mathbf{u} = \mathbf{f}, \\
                  \quad & g_{iso}(\mathbf{C}^H_{uc}) \leq 0, \\
                  \quad & g_{stiff}(\mathbf{C}^H_{uc}) \leq 0, \\
                  \quad & \frac{V}{V_0 f} - 1 \leq 0, \\
                  \quad & \mathbf{0} \leq \mathbf{x} \leq \mathbf{1}
\end{align*}
$$
where
$$
\begin{align*}
g_{stiff}(\mathbf{C}_{uc}^H) &= 1 - \frac{C_{11}^H + C_{22}^H}{2C_0} \\ 
C_0 &= C^\ast (C_{11}^H)_{tri}  =  C^\ast \frac{3Ew}{8}\bar{\rho}_{uc}
\end{align*}
$$
and $f$ is computed from the physical relative density of the unit cell as:

$$
\bar{\rho}_{uc} = \frac{S_{uc}^0}{S_{uc}}f  \quad \Rightarrow  \quad f  = \frac{S_{uc}}{S_{uc}^0} \bar{\rho}_{uc}
$$
where $S_{uc}^0 = t_{max}L_{uc}^{tot}$ is the maximum surface area if all struts are solid, and $S_{uc} = |\mathbf{a}_1 \times \mathbf{a}_2 |$ is the surface area of the unit cell.

::right::
Relative element density:
$$ \rho_e(x_e) = \rho_{\min} + x_e^{q_k}(1 - \rho_{\min}), \qquad x_e \in [0, 1] $$
Stiffness interpolation using relative element density:
$$
\mathbf{K}(\mathbf{x}) = \sum_{e=1}^{N_e} \rho_e(x_e) \mathbf{K}_e^0
$$

Stress *interpolation* gives the relaxed stress $\tilde{\sigma}_e$ as
$$
\tilde{\sigma}_e = x_e^{q_\sigma} \sigma_e 
$$
where $\sigma_e$ is the maximum fiber stress for a solid element $e$, i.e. $\rho_e = 1$.

$N_{uc} = 2 \hspace{40mm} N_{uc}=3$ 
<div class="grid grid-cols-2 gap-4">
  <div>
    <img src="/media/unit_cell_2x2_white.png" style="width:300px"/>
  </div>
  <div>
    <img src="/media/unit_cell_3x3_white.png" style="width:300px"/>
  </div>
</div>


---
layout: two-cols-header
zoom: .8
---

## Fracture energy optimization - load control

$\bar{\rho} = 0.0625, \ p = 4, \ N_{uc} = 2$


Full stiffness fraction: $C^\ast = 1.0$, and stiffness penalization:

$
q_k = 
\begin{cases}
1.25 & \text{for } i \in [0, 49]  \\ 
1.50 & \text{for } i \in [50, 99]  \\ 
\end{cases}
$


::left::

<figure style="position:relative; top: 20px; left:0px; display: table" >
  <SlidevVideo muted autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:600px">
    <source src="/media/triangular_test/UnitCell_le_0.062_vfrac_0.06_cmp.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 


:: right :: 

<figure style="position:relative; top: 20px; left:20px; display: table" >
  <SlidevVideo muted autoreset="click" autoplay 
  style="position:relative; top:0px; left:0px; width:600px">
    <source src="/media/triangular_test/UnitCell_le_0.062_vfrac_0.06_cmp_stress.mp4" type="video/mp4">
  </SlidevVideo> 
</figure> 

<img src="/media/triangular_test/UnitCellGrid_designHistory_00099.png" 
     style="position:fixed; top:20px; right:20px; width:550px"/>

