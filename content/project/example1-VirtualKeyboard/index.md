---
title: Eye-Controlled Virtual Keyboard Layout Quantitative Design System
summary: Conducting ergonomic experiments to investigate whether the keyboard layout (especially its similarity to the QWERTY layout) would affect gaze-typing performance.
tags:
  - Research
date: '2021-05-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Center
  preview_only: true

links:
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example

---
## Introduction

Using eye-tracking for typing is like clicking keys one by one with a single finger. We were curious about whether the keyboard layout (especially its similarity to the QWERTY layout) would affect typing performance.

Inspired by some papers related to the Quantitative Design of Virtual Keyboard Layout [^1] [^2] [^3] by Prof. Shumin Zhai, we conducted Monte Carlo simulations to create 5 virtual keyboard layouts with varying degrees of similarity to the QWERTY layout. 

![image](2.jpg "5 virtual keyboard layouts")

We designed two typing tasks, "Word Input" and "Phrase Input," and invited 15 participants to take part in the experiment. The results indicate that the more similar a layout is to the QWERTY layout, the better the users' performance, regardless of whether they are beginners or experts in eye-tracking devices.

![image](1.jpg "A participant in the experiment")

![image](Show.jpg "The experiment procedure")

As the project leader, I collaborated with an undergraduate student, and my main responsibilities included:
- Generating the project idea and developing the research scheme.
- Assisting in proposing the layout generation algorithm based on the Monte Carlo Method.
- Creating an experimental platform using Unity and the Tobii Eye Tracker API.
- Guiding the undergraduate student in conducting experiments and analyzing the results through SPSS.


---

### Reference

[^1]: Zhai, S., Hunter, M., & Smith, B. A. (2000, November). The metropolis keyboard-an exploration of quantitative techniques for virtual keyboard design. In Proceedings of the 13th annual ACM symposium on User interface software and technology (pp. 119-128).

[^2]: Bi, X., Smith, B. A., & Zhai, S. (2010, April). Quasi-qwerty soft keyboard optimization. In Proceedings of the SIGCHI Conference on Human Factors in Computing Systems (pp. 283-286).

[^3]: Bi, X., & Zhai, S. (2016, May). IJqwerty: What difference does one key change make? Gesture typing keyboard optimization bounded by one key position change from Qwerty. In Proceedings of the 2016 CHI Conference on Human Factors in Computing Systems (pp. 49-58).

---
