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
{{< figure src="images/series-circuit.jpg" title="All resistors = $5\Omega$" lightbox="false" >}}

{{% fragment %}} $V_{Batt}$ {{% /fragment %}} {{% fragment %}} $- V_3$ {{% /fragment %}} {{% fragment %}} $- V_2$ {{% /fragment %}} {{% fragment %}} $- V_1 = 0$ {{% /fragment %}}

We know V = IR, so 

{{% fragment %}} $V_{Batt}$ {{% /fragment %}} {{% fragment %}} $- I_3R_3$ {{% /fragment %}} {{% fragment %}} $- I_2R_2$ {{% /fragment %}} {{% fragment %}} $- I_1R_1 = 0$  {{% /fragment %}}

---
{{< figure src="images/series-circuit.jpg" title="All resistors = $5\Omega$" lightbox="false" >}}

$V_{Batt} - I_3R_3 - I_2R_2- I_1R_1 = 0$ and current is the same everywhere in a series circuit...so

{{% fragment %}} $V_{Batt} - I(R_3 + R_2 + R_1) = 0${{% /fragment %}}
---

---

## Features

- Efficiently write slides in Markdown
- 3-in-1: Create, Present, and Publish your slides
- Supports speaker notes
- Mobile friendly slides

---




---

## Fragments

Make content appear incrementally

```
{{%/* fragment */%}} One {{%/* /fragment */%}}
{{%/* fragment */%}} **Two** {{%/* /fragment */%}}
{{%/* fragment */%}} Three {{%/* /fragment */%}}
```

Press `Space` to play!

{{% fragment %}} One {{% /fragment %}}
{{% fragment %}} **Two** {{% /fragment %}}
{{% fragment %}} Three {{% /fragment %}}

---

A fragment can accept two optional parameters:

- `class`: use a custom style (requires definition in custom CSS)
- `weight`: sets the order in which a fragment appears

---

## Speaker Notes

Add speaker notes to your presentation

```markdown
{{%/* speaker_note */%}}
- Only the speaker can read these notes
- Press `S` key to view
{{%/* /speaker_note */%}}
```

Press the `S` key to view the speaker notes!

{{< speaker_note >}}
- Only the speaker can read these notes
- Press `S` key to view
{{< /speaker_note >}}

---

## Themes

- black: Black background, white text, blue links (default)
- white: White background, black text, blue links
- league: Gray background, white text, blue links
- beige: Beige background, dark text, brown links
- sky: Blue background, thin dark text, blue links

---

- night: Black background, thick white text, orange links
- serif: Cappuccino background, gray text, brown links
- simple: White background, black text, blue links
- solarized: Cream-colored background, dark green text, blue links

---

{{< slide background-image="/img/boards.jpg" >}}

## Custom Slide

Customize the slide style and background

```markdown
{{</* slide background-image="/img/boards.jpg" */>}}
{{</* slide background-color="#0000FF" */>}}
{{</* slide class="my-style" */>}}
```

---

## Custom CSS Example

Let's make headers navy colored.

Create `assets/css/reveal_custom.css` with:

```css
.reveal section h1,
.reveal section h2,
.reveal section h3 {
  color: navy;
}
```

---

# Questions?

[Ask](https://spectrum.chat/academic)

[Documentation](https://sourcethemes.com/academic/docs/managing-content/#create-slides)
