---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title:  
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.

    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false


  - block: collection
    id: collection
    content:
      title: Publications
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


  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
