---
title: Ch 19 Slides
summary: A basic overview of Ch 19 from Chabay and Sherwood.
authors: []
tags: []
categories: []
date: "2019-02-05T00:00:00Z"
slides:
  # Choose a theme from https://github.com/hakimel/reveal.js#theming
  theme: white
  # Choose a code highlighting style (if highlighting enabled in `params.toml`)
  #   Light style: github. Dark style: dracula (default).
  highlight_style: dracula
---

### Resistors and Capacitors

**Resistors**
- Conductors that have different resistivity
- Resistivity, $\rho = \frac{\left| \vec{E} \right| }{J} = R\frac{A}{l}$
- $R = \frac{\rho l}{A}$

**Capcitors**
- Most simply, plates that allow charges to distribute over their area. 
- Capacitance, $C = \epsilon_0 \frac{A}{d}$

---

### Loop Rule

$\Sigma V = 0$ 
Around any closed loop

---
### Series Circuits
{{< figure src="images/series-circuit.jpg" >}}

{{% fragment %}} $V_{Batt}$ {{% /fragment %}} {{% fragment %}} $- V_3$ {{% /fragment %}} {{% fragment %}} $- V_2$ {{% /fragment %}} {{% fragment %}} $- V_1 = 0$ {{% /fragment %}}

{{% fragment %}} We know V = IR, so {{% /fragment %}}

{{% fragment %}} $V_{Batt}$ {{% /fragment %}} {{% fragment %}} $- I_3R_3$ {{% /fragment %}} {{% fragment %}} $- I_2R_2$ {{% /fragment %}} {{% fragment %}} $- I_1R_1 = 0$  {{% /fragment %}}

---
### Series Circuits
{{< figure src="images/series-circuit.jpg" >}}

$V_{Batt} - I_3R_3 - I_2R_2- I_1R_1 = 0$ 

I is the same everywhere in a series circuit

{{% fragment %}} $V_{Batt} - I(R_3 + R_2 + R_1) = 0${{% /fragment %}}

---
### Series Circuits
{{< figure src="images/series-circuit.jpg" >}}

$V_{Batt} - I(R_3 + R_2 + R_1) = 0$ 

In series circuits, then...
{{% fragment %}} $V_{Batt} - IR_{Total} = 0$ {{% /fragment %}}

{{% fragment %}} $R_{Total} = R_1 + R_2 + R_3+...$ {{% /fragment %}}

---
### Parallel Circuits
{{< figure src="images/Parallel.png" >}}

Choose a path $1 \rightarrow 8 \rightarrow 7 \rightarrow 2 \rightarrow 1$, then,

{{% fragment %}} $V_{Batt} - I_1R_1 = 0$ {{% /fragment %}}

---
### Parallel Circuits
{{< figure src="images/Parallel.png" width="300px">}}

Choose a different path $1 \rightarrow 8 \rightarrow 6 \rightarrow 3 \rightarrow 1$

{{% fragment %}} $V_{Batt} - I_2R_2 = 0$ {{% /fragment %}}

---
### Parallel Circuits
{{< figure src="images/Parallel.png" width="300px">}}
Since $V_{Batt} - I_2R_2 = 0$ and $V_{Batt} - I_2R_2 = 0$

In each branch of a parallel circuit, $\Delta V$ must be the same.

{{% fragment %}} $V_1 = V_2 = V_3 = V_{Batt}$ {{% /fragment %}}

---
### Parallel Circuits
In a parallel circuit, the current splits at each junction. So the current leaving the battery is $I_{Total} = I_1 + I_2 + I_3$

And, $V = IR$ or $I = V/R$ which can be substituted in.

$$I_{Total} = V_1/R_1 + V_2/R_2 + V_3/R_3$$

---
### Parallel Circuits
$$I_{Total} = V_1/R_1 + V_2/R_2 + V_3/R_3$$
But, V is same across all parallel branches, so

$$V/R_{Total} = V/R_1 + V/R_2 + V/R_3$$
$$V/R_{Total} = V(1/R_1 + 1/R_2 + 1/R_3)$$

In Parallel branches
$$1/R_{Total} = 1/R_1 + 1/R_2 + 1/R_3 + ...$$

---
*Series Circuits*
Current is same at all points
$$ \Sigma \Delta V = 0$$
$R_{Total} = R_1 + R_2 + R_3+...$

*Parallel Circuits*
Voltage is same across all branches
$$I_{Total} = I_1 + I_2 + I_3$$
$1/R_{Total} = 1/R_1 + 1/R_2 + 1/R_3 + ...$

---


### Capacitors
{{< youtube Guhao1KxaPc >}}

---

### Capacitors
{{< figure src="images/RCCircuit.png" width="300px">}}
**Charging Capacitor** 

As capacitor charges, charge builds up on plates of capacitor, creating electric field, building up a potential difference across the capacitor.


---

### Capacitors
{{< figure src="images/RCCircuit.png" width="300px">}}

**Charging Capacitor** 

Charge on capacitor: $Q = VC$

Capacitance: $C = \epsilon (A/d)$

---
### Capacitors - Charging
{{< figure src="images/RCCircuit.png" width="300px">}}

Loop rule still applies, so 

{{% fragment %}} $V_{Batt}$ {{% /fragment %}}
{{% fragment %}} $-V_{Cap}$ {{% /fragment %}}
{{% fragment %}} $-V_{Res} = 0$ {{% /fragment %}}


---
### Capacitors - Charging

$$V_{Batt} -V_{Cap} -V_{Res} = 0$$

{{% fragment %}} $$V_{Batt} -Q/C - IR = 0$$ {{% /fragment %}}

{{% fragment %}} $$V_{Batt} -Q(t)/C - \frac{dQ(t)}{dt}R = 0$$ {{% /fragment %}}

---
### Capacitors - Charging
  
$$V_{Batt} -Q(t)/C - \frac{dQ(t)}{dt}R = 0$$
  
- Look at the initial and final conditions.
    - At $t = 0, I = I_0, Q = Q_0, Q_0 often = 0 $
    - As $t \rightarrow \infty, I \rightarrow 0, Q \to VC$
    
{{% fragment %}} $Q(t) = Q_0(1- e^{-t/RC})$ {{% /fragment %}}
    
---

At time = 0 
$$Q(t) = Q_0(1- e^{-t/RC})$$
$$\frac{dQ(t)}{dt} = \frac{Q_0}{RC}e^{-t/RC}$$
at t = 0, $Q(0) = Q_0$,  and $I_0 = \frac{Q_0}{RC} = V/R$

---

As time goes to infinity
$$Q(t) = Q_0(1- e^{-t/RC})$$
$$\frac{dQ(t)}{dt} = \frac{Q_0}{RC}e^{-t/RC}$$
as $t \to \infty, Q(\infty) = VC$, and $I(\infty) = I_0(1-1) = 0$

---
### Capacitors - Disharging
{{< figure src="images/RC.jpg">}}

Loop rule still applies, so 

{{% fragment %}} $V_{Cap}$ {{% /fragment %}}
{{% fragment %}} $-V_{Res} = 0$ {{% /fragment %}}
 
---

### Capacitors - Disharging
  $$V_{Cap} -V_{Res} = 0$$

  {{% fragment %}} $$Q/C - IR = 0$$ {{% /fragment %}}
  
  {{% fragment %}} $$Q(t)/C - \frac{dQ(t)}{dt}R = 0$$ {{% /fragment %}}

---
### Capacitors - Disharging
  
$$Q(t)/C - \frac{dQ(t)}{dt}R = 0$$
  
- Look at the initial and final conditions.
    - At $t = 0, I = I_0, Q_0 = VC$
    - As $t \to \infty, I \to 0, Q \to 0$
    
{{% fragment %}} $Q(t) = VCe^{-t/RC}$ {{% /fragment %}}
    
---

At time = 0 
$$Q(t) = VCe^{-t/RC}$$
$$\frac{dQ(t)}{dt} = \frac{VC}{-RC}e^{-t/RC}$$
at t = 0, $Q(0) = VC$,  and $I_0 = -\frac{VC}{RC} = -V_{C}/R$

---


As time goes to infinity
$$Q(t) = VCe^{-t/RC}$$
$$\frac{dQ(t)}{dt} = \frac{VC}{-RC}e^{-t/RC}$$
as $t \to \infty, Q(\infty) = 0$, and $I(\infty) = V_{C}/R = 0$

---