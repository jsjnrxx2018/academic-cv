---
title: ''
summary: ''
date: 2022-10-24
type: landing

sections:

  # =======================
  # 1. 个人介绍
  # =======================
  - block: resume-biography-3
    content:
      username: me
      text: ''
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: About
        education: Education
        interests: Interests
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: lg
      avatar:
        size: medium
        shape: circle

  # =======================
  # 2. 研究简介
  # =======================
  - block: markdown
    content:
      title: '📚 Research Overview'
      text: |
        Welcome to my academic website.

        My research focuses on:
        - Computer Vision
        - Vision-Language Models
        - Plant Disease Recognition
        - Anomaly Detection
        - Open-World Learning

        Feel free to explore my work below.
    design:
      columns: '1'

  # =======================
  # 3. Publications（稳定版）
  # =======================
  - block: collection
    id: papers
    content:
      title: Publications
      filters:
        folders:
          - publications
        featured_only: false
    design:
      view: article-grid
      columns: 2

  # =======================
  # 4. Recent Publications（关键修复）
  # =======================
  - block: collection
    content:
      title: Recent Publications
      filters:
        folders:
          - publications
    design:
      view: article-grid   # ❗避免 citation bug

  # =======================
  # 5. Talks
  # =======================
  - block: collection
    id: talks
    content:
      title: Talks
      filters:
        folders:
          - events
    design:
      view: card

  # =======================
  # 6. Blog / News
  # =======================
  - block: collection
    id: news
    content:
      title: News
      page_type: blog
      count: 6
      filters:
        exclude_featured: false
        exclude_future: false
    design:
      view: card

  # =======================
  # 7. CTA（可选）
  # =======================
  - block: markdown
    content:
      title: '🚀 Contact'
      text: |
        If you are interested in collaboration, feel free to contact me.
    design:
      columns: '1'

---
