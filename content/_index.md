---
# Leave the homepage title empty to use the site title
title:
date: 2023-10-23
type: landing

image: icon.png

sections:
  - block: about.biography
    id: about
    content:
      title: Biografía
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: collection
    id: posts
    content:
      title: Dat4 Lab
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
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
  - block: collection
    id: featured
    content:
      title: ABC Lab
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: compact
  - block: contact
    id: contact
    content:
      title: Contacto
      subtitle:
      text: |-
        Puede comunicarse conmigo por este medio y estare repondiendo su consulta lo mas pronto posible
      # Contact (add or remove contact options as necessary)
      email: nuno.pgarcia@gmail.com
      phone: +584120442730
      contact_links:
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: true
    design:
      columns: '2'
---
