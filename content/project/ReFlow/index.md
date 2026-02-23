---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "ReFlow"
summary: "ReFlow extracts floating-point C code from a PVS real numbers specification.
The code is annotated with ACSL pre- and post-conditions that bound the accumulated round-off error.<br>
ReFlow can also instrument the C code to detect when the floating-point control flow diverges with respect to the ideal real numbers' one.
"
authors: [Laura Titolo, Mariano M. Moscato, Marco A. Feliu, Cesar A. Muñoz, Aaron Dutle]
tags: []
categories: []
date: 2024-09-09T15:13:57-04:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- name: Code
  url: https://github.com/nasa/PRECiSA
  icon_pack: fab
  icon: github

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
ReFlow extracts floating-point C code from a PVS real numbers specification. The code is annotated with ACSL pre- and post-conditions that bound the accumulated round-off error.

ReFlow can also instrument the C code to detect when the floating-point control flow diverges with respect to the ideal real numbers' one.
