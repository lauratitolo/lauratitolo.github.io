---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      # button:
      #   text: Download CV
      #   url: static/uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  # - block: markdown
  #   content:
  #     title: '📚 My Research'
  #     subtitle: ''
  #     text: |-
  #       My research focuses on different aspects and applications of formal methods.<br>
  #       At <b>NASA</b> I was developing new tools for the formal verification and analysis of safety-critical avionics applications. In particular, I developed and applied rigorous techniques for improving the reliability of airspace software involving finite-precision computations.
  #       I was the main developer of the [PRECiSA](https://github.com/nasa/PRECiSA) round-off error static analyzer for floating-point programs and the [ReFlow](https://github.com/nasa/reflow) floating-point C code extractor. 
  #       In addition, I contributed to different PVS libraries for structured natural language requirements, hybrid systems' verification, and temporal logics.<br>
  #       At <b>Code Metal</b> I am applying formal verification techniques to improve the quality of automatically transpiled code for edge computing. 
  #   design:
  #     columns: '2'
  # - block: markdown
  #   content:
  #     title: '📋 Service'
  #     subtitle: ''
  #     text: |-
  #         I am an active member of the formal methods and programming languages communities, and I have served as program committee chair and member in several international conferences.
  #         #### Upcoming events:
  #           - [NFM 2025](https://shemesh.larc.nasa.gov/nfm2025/) (General   Chair),
  #           - LOPSTR 2025 (PC co-chair),
  #           - [CPP 2025](https://popl25.sigplan.org/home/CPP-2025) (PC),
  #           - [PADL 2025](https://popl25.sigplan.org/home/PADL-2025)(PC)
  #         #### Past Events:
  #         [NSAD 2024](https://2024.splashcon.org/home/nsad-2024) (PC),
  #         [FMICS 2024](https://fmics.inria.fr/2024/) (PC),
  #         [LOPSTR 2024](https://lopstr.github.io/2024/) (PC),
  #         [ARITH 2024](https://www.ac.uma.es/arith2024/index.html) (PC),
  #         [SAS 2023](https://conf.researchr.org/home/sas-2023) (PC),
  #         [ARITH 2023](https://arith2023.arithsymposium.org) (PC),
  #         [LOPSTR 2023](https://lopstr.github.io/2023/) (PC)
  #         [NFM 2023](https://conf.researchr.org/home/nfm-2023) (PC)
  #         [SAS 2022](https://2022.splashcon.org/home/sas-2022#Home) (PC),
  #         [LOPSTR 2022](https://lopstr2022.webs.upv.es) (PC),
  #         [SOAP 2022](https://pldi22.sigplan.org/home/SOAP-2022) (PC   co-chair),
  #         [CAV 2022](http://i-cav.org/2022/) (PC)
  #         [VMCAI 2022](https://popl22.sigplan.org/home/VMCAI-2022) (PC),
  #         [CPP 2022](https://popl22.sigplan.org/home/CPP-2022) (PC),
  #         [SOAP 2021](https://pldi21.sigplan.org/home/SOAP-2021) (PC),
  #         [FMAS 2021](https://fmasworkshop.github.io/FMAS2021/) (PC),
  #         [ESEC/FSE 2021](https://2021.esec-fse.org) (PC Demonstration   track),
  #         [DETECT 2021](https://detect.ensma.fr/2021/) (PC)
  #         [NFM 2021](https://shemesh.larc.nasa.gov/nfm2021/) (PC co-chair),
  #         [NSV 2020](https://nsv2020.github.io) (PC),
  #         [NFM 2020](https://ti.arc.nasa.gov/events/nfm-2020/) (PC),
  #         [FMAS 2020](https://fmasworkshop.github.io/FMAS2020/) (PC),
  #         [DETECT 2020](https://detect.ensma.fr/2020/) (PC),
  #         [NSV 2019](https://nsv19.mpi-sws.org) (PC),
  #         [TNC 2018](https://perso.univ-perp.fr/nasrine.damouche/TNC%2718/)   (PC),
  #         [NSV 2018](https://nsv-2018.github.io/nsv2018/committee.html)   (PC),
  #         [NFM 2018](https://shemesh.larc.nasa.gov/NFM2018/) (PC)
  
  #   design:
  #     columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: projects
    content:
      title: Projects
      text: ""
      filters:
        folders:
          - project
        exclude_featured: false
    design:
      view: cards
  - block: resume-experience
    id: experience
    content:
      title: Experience
      text: "" 
      design:
        view: title-summary
      filters:
        folders:
          - experience  
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

        Easily build anything with blocks - no-code required!
        
        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
