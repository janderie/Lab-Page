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
        
         Professor Anderies' Lab group's current research interests focus on robust management and robust institutional design for coupled social-ecological systems. Other areas of interest include economic growth, demographics, migration, environmental justice, and inequality. This is the latest.
         {style="color: red"}
         
    design:
      background:
        image: 
          filename: stacked-peaks.svg
          filters:
            brightness: 1
          parallax: false
          position: center
          size: cover
         

  
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
      view: card
      columns: '1'


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
        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
    design:
      columns: '1'
---
