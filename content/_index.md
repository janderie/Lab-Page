---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      image:
        filename: welcome_1.png
      text: |
        <br>
        
         Our research focuses on the interplay between institutions, decision-making and the environment in an effort to inform robust institutional design for coupled social-ecological-technical systems. Other areas of interest include economic growth, demographics, migration, environmental justice, and inequality.
         {style="line-height:1.4"} 
    design:
      background:
      # Choose colors such as from https://html-color-codes.info
      gradient_start: '#4bb4e3'
      gradient_end: '#2b94c3'
      # The gradient angle from 0-360 degrees
      gradient_angle: 180
      # Text color (true=light, false=dark, or remove for the dynamic theme color).
      text_color_light: true
  
  - block: collection
    content:
      title: Latest News
      subtitle:
      text:
      count: 5
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: post
    design:
      view: showcase


#Examples of different blocks, not used on landing page.

#general markdown block.... not used 
  #- block: markdown
   # content:
    #  title:
    #  subtitle: ''
    #  text:
    #design:
    #  columns: '1'
    #  background:
    #    image: 
    #      filename: coders.jpg
    #      filters:
    #        brightness: 1
    #      parallax: false
    #      position: center
    #      size: cover
    #      text_color_light: true
    #  spacing:
    #    padding: ['20px', '0', '20px', '0']
    #  css_class: fullscreen

  #- block: collection
   # content:
    #  title: Latest Preprints
    #  text: ""
    #  count: 5
    #  filters:
     #   folders:
     #     - publication
     #   publication_type: 'article'
    #design:
     # view: citation
     # columns: '1'

  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="./people/" cta_text="Meet the Lab Group →" %}}
    design:
      columns: '1'
---
