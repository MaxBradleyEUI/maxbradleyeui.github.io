---
# Home page
title: ""
date: 2022-10-24
type: landing

design:
  spacing: "6rem"

sections:
  - block: markdown
    content:
      title: "About Me"
      subtitle: ""
      text: |-
        **Max Bradley**

        PhD Researcher, [European University Institute](https://www.eui.eu)  
        Junior Visiting Scholar, [Nuffield College, University of Oxford](https://www.nuffield.ox.ac.uk/)

        I study the political economy of the green transition, focusing on how local human capital shapes adaptation and political responses.  
        Contact: [max.bradley@eui.eu](mailto:max.bradley@eui.eu)

    design:
      columns: "1"

  - block: markdown
    content:
      title: "📚 My Research"
      subtitle: ""
      text: |-
        Replace this paragraph with a short overview of your projects or current research.

    design:
      columns: "1"

  - block: collection
    id: papers
    content:
      title: "Featured Publications"
      filters:
        folders: ["publications"]
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    content:
      title: "Recent Publications"
      filters:
        folders: ["publications"]
        exclude_featured: false
    design:
      view: citation

  - block: collection
    id: talks
    content:
      title: "Recent & Upcoming Talks"
      filters:
        folders: ["events"]
    design:
      view: card

  - block: collection
    id: news
    content:
      title: "Recent News"
      page_type: blog
      count: 5
      order: desc
      filters:
        exclude_future: false
        exclude_past: false
    design:
      view: card
      spacing:
        padding: [0, 0, 0, 0]
---
