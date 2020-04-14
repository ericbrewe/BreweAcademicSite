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

## Loop Rule

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

Choose a path $1 \Rightarrow 8 \Rightarrow 7 \Rightarrow 2 \Rightarrow 1$, then,

{{% fragment %}} $V_{Batt} - I_1R_1 = 0$ {{% /fragment %}}

---
### Parallel Circuits
{{< figure src="images/Parallel.png" width = "50%">}}

Choose a different path $1 \Rightarrow 8 \Rightarrow 6 \Rightarrow 3 \Rightarrow 1$

{{% fragment %}} $V_{Batt} - I_2R_2 = 0$ {{% /fragment %}}

---
### Parallel Circuits
Since $V_{Batt} - I_2R_2 = 0$ and $V_{Batt} - I_2R_2 = 0$

In each branch of a parallel circuit, $\DeltaV$ must be the same.

{{% fragment %}} $V_1 = V_2 = V_3 = V_{Batt}$ {{% /fragment %}}

---
### Parallel Circuits
In a parallel circuit, the current splits at each junction. So the current leaving the battery is $I_{Total} = I_1 + I_2 + I_3$

And, $V = IR$ or $I = V/R$ which can be substituted in.

$$I_{Total} = V_1/R_1 + V_2/R_2 + V_3/R_3$$

---


