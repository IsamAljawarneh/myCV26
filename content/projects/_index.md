---
title: 'Projects'
date: 2024-05-19
type: landing

design:
  # Section spacing
  spacing: '5rem'

# Page sections
sections:
  - block: collection
    content:
      title: Selected Projects
      text: |-
        <style>
        @keyframes projects-highlight-flash {
          0%, 100% { background-color: #b7e9ff; }
          50% { background-color: #fff; }
        }

        .projects-experience-link {
          display: inline-block;
          padding: 0.1em 0.3em;
          animation: projects-highlight-flash 1.2s ease-in-out infinite;
        }

        @media (prefers-reduced-motion: reduce) {
          .projects-experience-link {
            animation: none;
            background-color: #b7e9ff;
          }
        }
        </style>
        I enjoy making things. Here are a selection of projects that I have worked on over the years. See <a class="projects-experience-link" href="https://isamaljawarneh.github.io/myCV26/experience/#projects">additional project experience in Highlights</a>.
      filters:
        folders:
          - projects
    design:
      view: article-grid
      fill_image: false
      columns: 3
      show_date: false
      show_read_time: false
      show_read_more: false
---
