---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: experience
    id: experience
    content:
      title: Professional Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Postdoctoral Researcher
          company: Sun Yat-sen University
          company_url: https://www.sysu.edu.cn/sysuen
          company_logo: sysu2
          location: Shenzhen, China
          date_start: '2022-10-01'
          date_end: ''
          description: |2-
              Projects include:
              * Chemical proteomic study of disulfide/diselenide probes
              * Self-assembly nano-PROTAC for synergetic photo-chemo-therapy
              * Biomedical application of black phosphorus
        - title: Postdoctoral Researcher
          company: City University of Hong Kong
          company_url: https://www.cityu.edu.hk/
          company_logo: cityu1
          location: Kowloon Tong, Hong Kong
          date_start: '2021-09-01'
          date_end: '2022-09-30'
          description: |2-
              Projects include:
              * Developing isoxazole group as a native photo-cross-linker for chemoproteomics
              * Self-assembly activatable photosensitizers for targeted cancer theranostics
    design:
      columns: '2'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
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
      view: compact
      columns: '2'
  - block: markdown
    id: gallery
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
    text: |-
          I'm delighted to collaborate with researchers worldwide to address important questions and make meaningful advancements. Feel free to contact me via email or social media.
      # Contact (add or remove contact options as necessary)
      email: ke.cheng@my.cityu.edu.hk
      phone: +1 267 999-9182
          contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/kecheng55'
      address:
        street: 66 Gongchang Rd
        city: Shenzhen
        region: Guangdong
        postcode: '518107'
        country: China
        country_code: CN

      # Automatically link email and phone or display as text?
      autolink: true
    design:
      columns: '2'
---
