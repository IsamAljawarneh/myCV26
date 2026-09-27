---
title: Teaching
description: Courses taught and student mentoring.
toc: true
keywords:
  - Teaching
  - Courses
  - Mentoring
---


## Teaching Experience
<style>
  @keyframes syllabus-note-flash {
    0%, 100% { opacity: 1; }
    50% { opacity: 0.35; }
  }

  .syllabus-note {
    color: green;
    font-family: Helvetica, monospace;
    animation: syllabus-note-flash 3s ease-in-out infinite;
  }

  main .prose:has(h3) {
    position: relative;
  }

  main .prose:has(h3)::before {
    position: absolute;
    top: 0.75rem;
    bottom: 0;
    left: 50%;
    width: 2px;
    background: #d1d5db;
    content: '';
    transform: translateX(-50%);
  }

  main .prose:has(h3) h3 {
    position: relative;
    box-sizing: border-box;
    width: 50%;
    margin: 0;
    padding: 0.65rem 2rem 0.65rem 0;
    font-size: 1.65rem;
    line-height: 1.25;
  }

  main .prose:has(h3) h3::before {
    position: absolute;
    top: 50%;
    right: -0.45rem;
    width: 0.75rem;
    height: 0.75rem;
    border: 3px solid white;
    border-radius: 999px;
    background: #16a34a;
    box-shadow: 0 0 0 2px #16a34a;
    content: '';
    transform: translateY(-50%);
  }

  main .prose:has(h3) h3:nth-of-type(even) {
    margin-left: 50%;
    padding-right: 0;
    padding-left: 2rem;
  }

  main .prose:has(h3) h3:nth-of-type(even)::before {
    right: auto;
    left: -0.45rem;
  }

  main .prose:has(h3) h3 + p,
  main .prose:has(h3) h3 + details,
  main .prose:has(h3) h3 + p + details {
    box-sizing: border-box;
    width: 50%;
    margin-top: 0.75rem;
    margin-bottom: 0.75rem;
    padding-right: 2rem;
  }

  main .prose:has(h3) h3:nth-of-type(even) + p,
  main .prose:has(h3) h3:nth-of-type(even) + details,
  main .prose:has(h3) h3:nth-of-type(even) + p + details {
    margin-left: 50%;
    padding-right: 0;
    padding-left: 2rem;
  }

  main .prose:has(h3) .ubt-course-list {
    box-sizing: border-box;
    width: 50%;
    margin-left: 50%;
    padding-left: 2rem;
  }

  main .prose:has(h3) h3 + details,
  main .prose:has(h3) h3 + p + details {
    width: 100%;
    margin-left: 0;
    padding: 0;
  }

  main .prose:has(h3) h3 + details > summary,
  main .prose:has(h3) h3 + p + details > summary {
    box-sizing: border-box;
    width: 50%;
    padding-right: 2rem;
  }

  main .prose:has(h3) h3:nth-of-type(even) + details > summary,
  main .prose:has(h3) h3:nth-of-type(even) + p + details > summary {
    margin-left: 50%;
    padding-right: 0;
    padding-left: 2rem;
  }

  main .prose:has(h3) .ubt-course-list {
    width: 100%;
    margin-left: 0;
    padding-left: 0;
  }

  main .prose:has(h3) .ubt-course-list details > summary {
    box-sizing: border-box;
    width: 50%;
    margin-left: 50%;
    padding-left: 2rem;
  }

  main .prose:has(h3) details[open] > :not(summary) {
    max-width: none;
  }

  @media (max-width: 640px) {
    main .prose:has(h3)::before {
      left: 0.45rem;
      transform: none;
    }

    main .prose:has(h3) h3,
    main .prose:has(h3) h3:nth-of-type(even) {
      width: auto;
      margin-left: 1.5rem;
      padding: 0.65rem 0 0.65rem 1rem;
      font-size: 1.35rem;
    }

    main .prose:has(h3) h3::before,
    main .prose:has(h3) h3:nth-of-type(even)::before {
      right: auto;
      left: -1.5rem;
    }

    main .prose:has(h3) h3 + p,
    main .prose:has(h3) h3 + details,
    main .prose:has(h3) h3 + p + details,
    main .prose:has(h3) h3:nth-of-type(even) + p,
    main .prose:has(h3) h3:nth-of-type(even) + details,
    main .prose:has(h3) h3:nth-of-type(even) + p + details {
      width: auto;
      margin-left: 1.5rem;
      padding-right: 0;
      padding-left: 1rem;
    }

    main .prose:has(h3) .ubt-course-list {
      width: auto;
      margin-left: 1.5rem;
      padding-left: 1rem;
    }

    main .prose:has(h3) h3 + details,
    main .prose:has(h3) h3 + p + details,
    main .prose:has(h3) .ubt-course-list {
      width: auto;
      margin-left: 1.5rem;
      padding-left: 1rem;
    }

    main .prose:has(h3) h3 + details > summary,
    main .prose:has(h3) h3 + p + details > summary,
    main .prose:has(h3) .ubt-course-list details > summary {
      width: auto;
      margin-left: 0;
      padding-right: 0;
      padding-left: 0;
    }
  }

  .teaching-table-wrap {
    margin: 1.5rem 0 2.5rem;
    overflow-x: auto;
  }

  .teaching-course-table {
    border-collapse: collapse;
    min-width: 48rem;
    table-layout: fixed;
    width: 100%;
  }

  .teaching-course-table th,
  .teaching-course-table td {
    border-bottom: 1px solid #d1d5db;
    padding: 1rem 0.9rem;
    text-align: left;
    vertical-align: top;
    overflow-wrap: anywhere;
  }

  .teaching-course-table th {
    color: #172033;
    font-size: 1.05rem;
    font-weight: 600;
  }

  .teaching-course-table th:nth-child(1),
  .teaching-course-table td:nth-child(1) { width: 32%; }

  .teaching-course-table th:nth-child(2),
  .teaching-course-table td:nth-child(2) { width: 16%; }

  .teaching-course-table th:nth-child(3),
  .teaching-course-table td:nth-child(3) { width: 27%; }

  .teaching-course-table th:nth-child(4),
  .teaching-course-table td:nth-child(4) { width: 25%; }

  .teaching-course-table a {
    text-decoration: underline;
    text-underline-offset: 0.15em;
  }

  .teaching-course-list {
    margin: 1.5rem 0 2.5rem;
  }

  .teaching-course-term {
    border-bottom: 1px solid #9db4c8;
    color: #2d617f;
    font-size: 1.15rem;
    letter-spacing: 0.28em;
    margin: 0 0 1.5rem;
    padding-bottom: 0.75rem;
    text-transform: uppercase;
  }

  .teaching-course-entry {
    border-bottom: 1px solid #d1dbe4;
    display: grid;
    gap: 1.5rem;
    grid-template-columns: 9rem 1fr;
    padding: 1.5rem 0;
  }

  .teaching-course-code {
    color: #315b77;
    font-size: 1.1rem;
  }

  .teaching-course-name {
    font-size: 1.5rem;
    line-height: 1.25;
    margin: 0;
  }

  .teaching-course-name a {
    text-decoration: underline;
    text-underline-offset: 0.12em;
  }

  .teaching-course-meta {
    color: #64748b;
    font-size: 1.1rem;
    line-height: 1.45;
    margin: 0.35rem 0 0;
  }

  .teaching-course-note {
    color: #475569;
    font-size: 0.95rem;
    margin: 0.5rem 0 0;
  }

  @media (max-width: 640px) {
    .teaching-course-table {
      min-width: 42rem;
    }

    .teaching-course-table th,
    .teaching-course-table td {
      padding: 0.8rem 0.65rem;
    }
  }

</style>
Levels: Undergraduate (UG) and Postgraduate (PG)

<p class="syllabus-note">Click a course title to read the syllabus.</p>

### 2022 - Present: Assistant Professor

{{< spoiler text="Open to see list of courses" >}}

**University of Sharjah, UAE**

<div class="teaching-course-list">
<h4 class="teaching-course-term">University of Sharjah</h4>
<article class="teaching-course-entry"><div class="teaching-course-code">1501330</div><div><h5 class="teaching-course-name">{{< staticref "uploads/syllabi/1501330_Introduction_to_Artificial_Intelligence.pdf" "newtab" >}}Introduction to AI{{< /staticref >}}</h5><p class="teaching-course-meta"><em>Undergraduate; Fall 2026/2027.</em></p></div></article>
<article class="teaching-course-entry"><div class="teaching-course-code">1501211</div><div><h5 class="teaching-course-name">{{< staticref "uploads/syllabi/1501211_Programming_II.pdf" "newtab" >}}Programming II{{< /staticref >}}</h5><p class="teaching-course-meta"><em>Undergraduate; Fall 2025/2026.</em></p></div></article>
<article class="teaching-course-entry"><div class="teaching-course-code">1501532</div><div><h5 class="teaching-course-name">{{< staticref "uploads/syllabi/1501532_GIS_Programming_Fundamentals.pdf" "newtab" >}}GIS Programming Fundamentals{{< /staticref >}}</h5><p class="teaching-course-meta"><em>Postgraduate (MSc); Fall 2024/2025 and Fall 2025/2026.</em></p></div></article>
<article class="teaching-course-entry"><div class="teaching-course-code">1501361</div><div><h5 class="teaching-course-name">{{< staticref "uploads/syllabi/1501361_Object_Oriented_Software_Design_and_Implementation.pdf" "newtab" >}}Object-Oriented Software Design and Implementation{{< /staticref >}}</h5><p class="teaching-course-meta"><em>Undergraduate; Fall 2024/2025.</em></p></div></article>
<article class="teaching-course-entry"><div class="teaching-course-code">1501247</div><div><h5 class="teaching-course-name">{{< staticref "uploads/syllabi/1501247_Multimedia_Programming_and_Design.pdf" "newtab" >}}Multimedia Design and Programming{{< /staticref >}}</h5><p class="teaching-course-meta"><em>Undergraduate; Fall 2023/2024 and Fall 2024/2025.</em></p></div></article>
<article class="teaching-course-entry"><div class="teaching-course-code">1501465</div><div><h5 class="teaching-course-name">{{< staticref "uploads/syllabi/1501465_Development_of_Web_Applications.pdf" "newtab" >}}Development of Web Applications{{< /staticref >}}</h5><p class="teaching-course-meta"><em>Undergraduate; Fall 2022/2023, Fall 2023/2024, Fall 2024/2025, and Fall 2025/2026.</em></p><p class="teaching-course-note">Updated the course materials.</p></div></article>
<article class="teaching-course-entry"><div class="teaching-course-code">1501394</div><div><h5 class="teaching-course-name">{{< staticref "uploads/syllabi/1501394_Junior_Project_in_CS.pdf" "newtab" >}}Senior Project{{< /staticref >}}</h5><p class="teaching-course-meta"><em>Undergraduate; Fall 2022/2023 and Fall 2023/2024.</em></p></div></article>
<article class="teaching-course-entry"><div class="teaching-course-code">N/A</div><div><h5 class="teaching-course-name">Web Programming</h5><p class="teaching-course-meta"><em>Undergraduate; Fall 2022/2023 and Fall 2023/2024.</em></p><p class="teaching-course-note">Updated the course materials.</p></div></article>
<article class="teaching-course-entry"><div class="teaching-course-code">N/A</div><div><h5 class="teaching-course-name">Programming for Engineers</h5><p class="teaching-course-meta"><em>Undergraduate; Fall 2022/2023 and Fall 2023/2024.</em></p></div></article>
<article class="teaching-course-entry"><div class="teaching-course-code">1501393</div><div><h5 class="teaching-course-name">{{< staticref "uploads/syllabi/1501393_Multimedia_Junior_Project.pdf" "newtab" >}}Junior Project{{< /staticref >}}</h5><p class="teaching-course-meta"><em>Undergraduate; Spring 2022/2023 and Spring 2023/2024.</em></p></div></article>
<article class="teaching-course-entry"><div class="teaching-course-code">1501564</div><div><h5 class="teaching-course-name">{{< staticref "uploads/syllabi/1501564_Foundations_of_Data_Science.pdf" "newtab" >}}Foundations of Data Science{{< /staticref >}}</h5><p class="teaching-course-meta"><em>Postgraduate (MSc); Spring 2022/2023, Spring 2023/2024, and Spring 2024/2025.</em></p><p class="teaching-course-note">Developed the course and designed the materials from scratch for the Data Science master's degree program.</p></div></article>
<article class="teaching-course-entry"><div class="teaching-course-code">N/A</div><div><h5 class="teaching-course-name">Introduction to IT</h5><p class="teaching-course-meta"><em>Undergraduate; Summer 2023, 2024, and 2025.</em></p></div></article>
</div>

{{< /spoiler >}}


### 2021/2022: Postdoctoral Research Fellow

**University of Bologna, Italy**
{{< spoiler text="Open to see list of courses" >}}

| Course | Level | Notes | Website |
|--------|-------|-------|---------|
| Designing Distributed Geospatial Data-Intensive Applications | PG (PhD) | Designed the course and created the course materials. | [Course page]({{< relref "PhD_course_2022" >}}) |

{{< /spoiler >}}

### 2017/2018: Teaching Assistant

**University of Bologna, Italy**
{{< spoiler text="Open to see list of courses" >}}
| Course | Level | Notes |
|--------|-------|-------|
| 37085 - Principles, Models and Applications for Distributed Systems M - LAB | PG (MSc) | Redesigned the course laboratory materials. |
{{< /spoiler >}}

### 2009 - 2016: University Lecturer

**University of Business and Technology, Saudi Arabia**

<style>
  .ubt-course-list summary {
    font-size: 1rem;
    font-weight: 400;
  }
</style>
<div class="ubt-course-list">
{{< spoiler text="Open to see list of courses" >}}
| Course | Level |
|--------|-------|
| [COE 201 - Computer Programming 1]({{< relref "IT201" >}}) | UG |
| [IT203 - Object-Oriented Computer Programming]({{< relref "IT203" >}}) | UG |
| [IT204 - Data Structures and Algorithms]({{< relref "IT204" >}}) | UG |
| [IT240 - Databases 1]({{< relref "IT240" >}}) | UG |
| [IT251 - Software Engineering 1]({{< relref "IT251" >}}) | UG |
| IT499 - Graduation Project | UG |
{{< /spoiler >}}
</div>
---

### Mentoring

#### Current Students

| Name | Program | Topic |
|------|---------|-------|
| Alice Smith | Ph.D. | Machine learning for scientific discovery |
| Bob Johnson | M.S. | Cloud computing optimization |

#### Past Students

{{< spoiler text="Graduated" >}}

| Name | Program | Topic | Year |
|------|---------|-------|------|
| Carol Williams | M.S. | Natural language processing | 2025 |
| David Brown | M.S. | Computer vision applications | 2024 |

{{< /spoiler >}}