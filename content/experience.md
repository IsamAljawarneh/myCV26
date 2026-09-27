---
title: 'Highlights'
date: 2026-09-19
type: landing

design:
  spacing: '5rem'

# Note: `username` refers to the user's folder name in `content/authors/`

# Page sections
sections:
  - block: markdown
    content:
      text: |-
        <p class="text-center">Full Resume in {{< staticref "uploads/resume.pdf" "newtab" >}}PDF{{< /staticref >}}.</p>
    design:
      columns: '1'
  - block: markdown
    content:
      title: Experience
      text: |-
        {{< experience-timeline >}}
    design:
      columns: '1'
  - block: markdown
    content:
      title: Funding
      text: |-
        <style>
        .funding-showcase { color: #1f2937; }
        .funding-entry { border-bottom: 1px solid #d6dce5; padding: 1.5rem 0 2.25rem; }
        .funding-entry + .funding-entry { padding-top: 2.25rem; }
        .funding-source { font-size: 1.9rem; line-height: 1.2; margin: 0 0 1.5rem; }
        .funding-source a, .funding-link { color: #3267b1; }
        .funding-label { background: #faf6e3; padding: 0.15rem 0.4rem; }
        .funding-title { font-size: 1.65rem; line-height: 1.45; margin: 0 0 1.5rem; }
        .funding-meta { font-size: 1.15rem; line-height: 1.8; margin: 0; }
        .funding-meta strong { color: #c73559; font-weight: 500; }
        .funding-meta .funding-label { color: #243447; }
        .funding-entry details { margin-top: 1.5rem; }
        .funding-entry summary { cursor: pointer; font-size: 1.15rem; list-style-position: outside; }
        .funding-entry details p { margin: 1rem 0 0 1.5rem; }
        @media (max-width: 640px) {
          .funding-source { font-size: 1.5rem; }
          .funding-title { font-size: 1.3rem; }
          .funding-meta, .funding-entry summary { font-size: 1rem; }
        }
        </style>
        <div class="funding-showcase">
        <article class="funding-entry">
        <h3 class="funding-source"><span class="funding-label">Microsoft</span> <a href="https://www.microsoft.com/en-us/ai/ai-for-earth">AI for Earth Fund</a></h3>
        <p class="funding-title"><em>Supporting Highly-Efficient Machine Learning Applications for Reducing the Impact of Climate Change on Human Health in Metropolitan Cities</em></p>
        <p class="funding-meta"><span class="funding-label">Role</span>: <strong>PI</strong><br><span class="funding-label">Period</span>: <strong>07/30/2020 - 07/30/2022</strong><br><span class="funding-label">Mentors</span>: <span class="funding-link">Prof.</span> <a class="funding-link" href="https://www.unibo.it/sitoweb/paolo.bellavista/en">Paolo Bellavista</a> &amp; <span class="funding-link">Prof.</span> <a class="funding-link" href="https://www.unibo.it/sitoweb/luca.foschini/en">Luca Foschini</a></p>
        <details>
        <summary>Click here to view the project description</summary>
        <p>The research project targets the challenge of reducing the adverse effects of climate changes on human health. Applications of Artificial Intelligence (AI) on spatially-tagged time-series human and vehicle mobility data to help in the efforts for reducing potential impacts of climate change.</p>
        </details>
        </article>
        <article class="funding-entry">
        <h3 class="funding-source"><span class="funding-label">Seed Research Project</span>, University of Sharjah</h3>
        <p class="funding-title"><em>Distributed Algorithms for Efficient Approximate Analytics of Multidimensional Big Data Streams</em></p>
        <p class="funding-meta"><span class="funding-label">Amount</span>: <strong>39,000 AED</strong><br><span class="funding-label">Period</span>: <strong>May 1, 2024 - May 1, 2026</strong><br><span class="funding-label">Collaborator</span>: <a class="funding-link" href="https://isamaljawarneh.github.io/myCV26/authors/madyan-omar-bagosher/">Madyan Omar Bagosher</a></p>
        <details>
        <summary>Click here to view the project summary</summary>
        <p>The project develops distributed online algorithms to summarize massive multidimensional IoT data streams in real time. Approximate aggregations balance accuracy and response time, enabling responsive visualizations such as city heatmaps to support urban planning.</p>
        </details>
        </article>
        <article class="funding-entry">
        <h3 class="funding-source"><span class="funding-label">Previous Funding</span></h3>
        <p class="funding-meta"><span class="funding-label">Fund source</span>: <a class="funding-link" href="https://www.ubt.edu.sa/About/Home">University of Business and Technology</a><br><span class="funding-label">Project title</span>: <em>a data warehouse for decision support at higher education</em><br><span class="funding-label">Role</span>: <strong>PI</strong><br><span class="funding-label">Period</span>: <strong>02/01/2015 - 12/30/2015</strong><br><span class="funding-label">Amount</span>: <strong>~$8000</strong></p>
        <details>
        <summary>Click here to view the project description</summary>
        <p>The project developed a higher-education data warehouse framework to support strategic planning and decision-making using real student data. It tailored warehouse design methods to university needs and showed how BI-driven analytics can improve institutional policy and planning.</p>
        </details>
        </article>
        </div>
    design:
      columns: '1'
  - block: markdown
    content:
      title: Professional Training
      text: |-
        <div class="w-full flex flex-col gap-6">
        <div class="w-full p-6 bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700">
        <h5 class="mb-2 text-2xl font-semibold text-gray-900 dark:text-white">3rd International Summer School on Deep Learning (DeepLearn 2019)</h5>
        <div class="block mb-3 text-sm font-normal leading-none text-gray-500 dark:text-gray-300">July 2019 · Warsaw, Poland</div>
        <p>Professional training in deep learning.</p>
        <a href="https://irdta.eu/deeplearn2019/">View training details</a>
        </div>
        <div class="w-full p-6 bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700">
        <h5 class="mb-2 text-2xl font-semibold text-gray-900 dark:text-white">Seventh European Business Intelligence &amp; Big Data Summer School (eBISS 2017)</h5>
        <div class="block mb-3 text-sm font-normal leading-none text-gray-500 dark:text-gray-300">July 2017 · Brussels, Belgium</div>
        <p>Presented a poster titled <em>QoS-Aware Big Geospatial Data Processing</em>.</p>
        <a href="https://cs.ulb.ac.be/conferences/ebiss2017/files/posters/aljawarneh_ebiss2017_poster.pdf">Download the poster PDF</a>
        </div>
        </div>
    design:
      columns: '1'
  - block: markdown
    content:
      title: Professional Memberships
      text: |-
        <div class="w-full flex flex-col gap-6">
        <div class="w-full p-6 bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700">
        <h5 class="mb-2 text-2xl font-semibold text-gray-900 dark:text-white">Institute of Electrical and Electronics Engineers (IEEE)</h5>
        </div>
        <div class="w-full p-6 bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700">
        <h5 class="mb-2 text-2xl font-semibold text-gray-900 dark:text-white">Institute of Advanced Studies (ISA), University of Bologna, Italy</h5>
        <div class="block mb-3 text-sm font-normal leading-none text-gray-500 dark:text-gray-300">2016 - 2020</div>
        </div>
        </div>
    design:
      columns: '1'
  - block: resume-skills
    content:
      title: Skills & Hobbies
      username: isam-mashhour-al-jawarneh
  - block: resume-awards
    content:
      title: Awards & Fellowships
      username: isam-mashhour-al-jawarneh
  - block: resume-languages
    content:
      title: Languages
      username: isam-mashhour-al-jawarneh
---
