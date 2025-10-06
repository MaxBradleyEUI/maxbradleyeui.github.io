---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  spacing: "6rem"

sections:
  # ✅ About block (pulls your author profile)
  - block: about
    content:
      title: ""
      author: admin
    design:
      avatar:
        size: medium
        shape: circle

  - block: markdown
    content:
      title: "📚 My Research"
      subtitle: ""
      text: |-
        Replace this with a short blurb about your research focus.

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
      text: ""
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
