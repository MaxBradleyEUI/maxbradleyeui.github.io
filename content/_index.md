---
# Home page
title: ""
date: 2022-10-24
type: landing

design:
  spacing: "6rem"

sections:
  # HERO (photo, name, socials, CV)
  - block: markdown
    id: hero
    content:
      title: ""
      subtitle: ""
      text: |-
        <div style="text-align:center; max-width:820px; margin: 0 auto;">
          <img src="/uploads/headshot_eui.jpg" alt="Max Bradley" style="width:220px;height:220px;border-radius:50%;object-fit:cover;margin:10px auto;display:block;">
          <h1 style="margin-top:10px;margin-bottom:8px;">Max Bradley</h1>
          <div style="font-size:1.1rem; line-height:1.5; margin-bottom:14px;">
            PhD Researcher, European University Institute
          </div>
          <div style="margin:14px 0;">
            <a href="mailto:max.bradley@eui.eu">Email</a> ·
            <a href="https://github.com/MaxBradleyEUI">GitHub</a> ·
            <a href="https://scholar.google.com/citations?user=4QegIYAAAAAJ&hl=en">Google Scholar</a> ·
            <a href="https://orcid.org/0009-0002-1750-3950">ORCID</a> ·
            <a href="https://www.linkedin.com/in/max-bradley/">LinkedIn</a> ·
            <a href="https://bsky.app/profile/maxbradley.bsky.social">Bluesky</a>
          </div>
          <div style="margin-top:6px;">
            <a href="/uploads/resume.pdf">Download CV</a>
          </div>
        </div>
    design:
      columns: "1"

  # About Me
  - block: markdown
    id: research
    content:
      title: "📚 About"
      subtitle: ""
      text: |-
        I study the political economy of the green transition. My work examines how local human capital concentration shapes firms’ adaptation to decarbonization and how these uneven economic effects translate into political preferences and behavior.
    design:
      columns: "1"

  # PUBLICATIONS (featured)
  - block: collection
    id: papers
    content:
      title: "Publications"
      filters:
        folders: ["publications"]
      featured_only: true
    design:
      view: article-grid
      columns: 2

  # TEACHING
  - block: collection
    id: teaching
    content:
      title: "Teaching"
      filters:
        folders: ["courses"]
      exclude_featured: false
    design:
      view: card
      columns: 2

  # NEWS / BLOG
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
