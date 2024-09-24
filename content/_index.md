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
          company: University of California San Francisco
          company_url: https://profiles.ucsf.edu/ke.cheng
          company_logo: UCSF
          location: San Francisco
          date_start: '2024-01-01'
          date_end: ''
          description: |2-
              Projects include:
              * Development of trioxolane antimalarials and anticancer drugs
              * Small-molecule probes for targeted radioligand therapy
        - title: Postdoctoral Researcher
          company: Sun Yat-sen University
          company_url: https://www.sysu.edu.cn/sysuen
          company_logo: sysu2
          location: Shenzhen
          date_start: '2022-10-01'
          date_end: '2023-12-01'
          description: |2-
              Projects include:
              * Self-assembly nano-PROTAC for synergetic photo-chemo-therapy
              * Black phosphorus nanomaterials for biomedical application
        - title: Postdoctoral Researcher
          company: City University of Hong Kong
          company_url: https://scholars.cityu.edu.hk/en/persons/ke-cheng(58c29bd6-cebe-40ed-acd8-7ed1cee38a13).html
          company_logo: cityu1
          location: Hong Kong
          date_start: '2021-09-01'
          date_end: '2022-09-30'
          description: |2-
              Projects include:
              * Isoxazole-based photo-cross-linker for photoaffinity labeling and chemoproteomics
              * Self-assembly activatable photosensitizers for cancer Nanotheranostics
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
      email: ke.cheng@ucsf.edu
      phone: 415-993-2020
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/kecheng55'
      address:
        street: 600 16th Street
        city: San Francisco
        region: California
        postcode: '94158'
        country: United States
        country_code: US
      # Automatically link email and phone or display as text?
      autolink: true
    design:
      columns: '2'
---
