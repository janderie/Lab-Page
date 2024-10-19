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
        
         Research in the Anderies Lab focuses on the interplay between institutions, decision-making and the environment in an effort to inform robust institutional design for coupled social-ecological-technical systems. Other areas of interest include economic growth, demographics, migration, environmental justice, and inequality.
         {style="line-height:1.4"}    
    #design:
     # background:
      #  image: 
       #   filename: hero_background.png
        #  filters:
         #   brightness: 0.9
          #parallax: true
          #position: center
          #size: cover

         
  
  - block: collection
    content:
      title: Latest Musings and News
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
