---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:


  - block: collection
    id: publication
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      columns: '2'
      view: citation

  - block: collection
    id: featured
    content:
      title: Software
      filters:
        folders:
          - project
        featured_only: false
    design:
      columns: '2'
      view: card
  
  - block: collection
    id: talks
    content:
      title: Guía para escribir un trabajo de fin de grado!
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
---
