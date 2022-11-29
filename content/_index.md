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
  - block: collection
    id: featured
    content:
      title: Featured Publications
      text:
      - '**Nowenstein**, I., Ingason, A.K. & Wallenberg, J. 2022. Conditioned Variation: Children Replicate Contrasts, not Parental Variant Rate. _University of Pennsylvania Working Papers in Linguistics_, 28(2), 14.'

      filters:
        folders:
          - publication
        featured_only: false
    design:
      columns: '2'
      view: card
  - block: collection
    id: talks
    content:
      title: Recent Talks & Posters
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
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
