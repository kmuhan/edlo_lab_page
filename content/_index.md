---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: markdown
    content:
      text: ' # Deep Learning Optimization Lab
      '
    design:
      columns: '1'

  - block: markdown
    content:
      text: '
<div style="margin: 10; display: flex; justify-content: center; align-items: center; height: 20vh;">
    <a href="research/deep-learning-sw-optimization" target="_blank" class="hover-effect" style="position: relative; display: inline-block; transition: transform 0.3s ease;">
        <img src="https://raw.githubusercontent.com/kmuhan/edlo_lab_page/refs/heads/main/images/screenshot.png" alt="Deep Learning SW Optimization" style="display: block;">
        <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); color: white; font-size: 24px; font-weight: bold; text-shadow: 1px 1px 5px black;">
            Deep Learning SW Optimization
        </div>
    </a>
    <a href="research/deep-learning-hardware-design" target="_blank" class="hover-effect" style="position: relative; display: inline-block; transition: transform 0.3s ease;">
        <img src="https://raw.githubusercontent.com/kmuhan/edlo_lab_page/refs/heads/main/images/screenshot.png" alt="Deep Learning Hardware Design" style="display: block;">
        <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); color: white; font-size: 24px; font-weight: bold; text-shadow: 1px 1px 5px black;">
            Deep Learning Hardware Design
        </div>
    </a>
</div>

<style>
    .hover-effect:hover {
        transform: scale(1.05); /* Slight zoom on hover */
    }
</style>
      '
    design:
      columns: '1'
  # - block: collection
  #   id: research
  #   content:
  #     filters:
  #       folders:
  #         - research
  #   design:
  #     view: masonry
  #     columns: '1'
  #     flip_alt_rows: true
  
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
  
  # - block: markdown
  #   content:
  #     title:
  #     subtitle: ''
  #     text:
  #   design:
  #     columns: '1'
  #     background:
  #       image: 
  #         filename: coders.jpg
  #         filters:
  #           brightness: 1
  #         parallax: false
  #         position: center
  #         size: cover
  #         text_color_light: true
  #     spacing:
  #       padding: ['20px', '0', '20px', '0']
  #     css_class: fullscreen

  - block: collection
    content:
      title: Latest Preprints
      text: ""
      count: 5
      filters:
        folders:
          - publication
        publication_type: 'article'
    design:
      view: citation
      columns: '1'
---
