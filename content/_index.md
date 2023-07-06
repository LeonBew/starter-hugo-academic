---
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title:  
      username: admin
  - block: portfolio
    id: projects
    content:
      title: Current Projects
      filters:
        folders:
          - project

    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false


  - block: collection
    id: collection
    content:
      title: Publications & Posts
      subtitle: ' '
      text: |-
      count: 0
      design:
        columns: '1'
      filters:
        # The folders to display content from
        folders:
          - publication
          - post


  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="pictures" resize_options="1024x1024" >}}
    design:
      columns: '1'
---
