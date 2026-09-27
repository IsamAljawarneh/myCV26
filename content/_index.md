---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: isam-mashhour-al-jawarneh
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        Isam Mashhour Al Jawarneh is an Assistant Professor of [Computer Science and Engineering](https://www.sharjah.ac.ae/Academics/College-of-Computing-and-Informatics) at [The University of Sharjah](https://www.sharjah.ac.ae/), where he leads research at the intersection of geospatial data science, big data systems, and AI for smart city analytics. He completed his Ph.D. in Computer Science and Engineering from [The University of Bologna](https://www.unibo.it/en), Italy, in 2020, and was a Postdoctoral Research Fellow there until 2022. Before that, he earned a Master’s degree in Information Technology and a B.Sc. in Computer Science, building a foundation in systems, data engineering, and applied computing.

        His research interests are in Geospatial Data Science, Big Data Management, and Intelligent Urban Analytics. His work aims to design scalable, real-time systems that can process massive spatiotemporal streams while preserving efficiency, accuracy, and decision-making value for cities, institutions, and public-health applications. The research spans three core areas:

        - **Geospatial Big Data Management**: building scalable architectures for ingesting, indexing, querying, and analyzing large-scale mobility, environmental, and urban data streams.
        - **Approximate and QoS-Aware Analytics**: designing adaptive methods that balance accuracy, latency, and computational cost for near-real-time geospatial decision support.
        - **AI for Smart Cities and Climate Resilience**: developing data-driven approaches that support urban planning, environmental monitoring, and health-aware analytics in complex metropolitan settings.

        We are actively looking for strong and motivated students and collaborators to join this research agenda. If you are interested in working with us, please get in touch and explore recent publications and projects.
    design:
      columns: '1'
  - block: team-showcase
    content:
      title: Meet the team
      subtitle: Geospatial AI, Big Data & Cloud Systems
      text: We develop scalable data and AI systems for intelligent, sustainable cities.
      user_groups:
        - Principal Investigators (faculty)
        - Researchers
      sort_by: name_family
      sort_ascending: true
      cta:
        text: Join us
        url: /myCV26/apply
        icon: hero/user-plus
    design:
      show_role: true
      show_organizations: true
      show_interests: true
      max_interests: 3
      show_social: true
      align: left
      max_columns: 3
      show_empty_groups: false
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - events
    design:
      view: card
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: card
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/kit" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/kit on GitHub">Star</a>

        Easily build anything with blocks - no-code required!

        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: 'bg-primary-300 dark:bg-primary-700'
        css_style: ''
  - block: markdown
    id: contact
    content:
      title: Contact
      text: |-
        I am open for collaboration. Contact me if you are working on any of the research topics that are related to my [research interests](#about).

        <div style="position: relative; width: 100%; aspect-ratio: 16 / 9; overflow: hidden;">
          <iframe src="https://www.google.com/maps/d/u/2/edit?mid=1ck0lFXOC8-uR2bRrQpvXqVTDU4Bri_s&usp=sharing" title="Interactive map" style="position: absolute; inset: 0; width: 100%; height: 100%; border: 0;" loading="lazy" allowfullscreen></iframe>
        </div>
    design:
      columns: '1'
---
