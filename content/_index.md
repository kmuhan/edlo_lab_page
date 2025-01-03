---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: markdown
    content:
      title:
      subtitle: ''
      text:
    design:
      columns: '1'
      background:
        image: 
          filename: EAIC_Logo1.png
          filters:
            brightness: 1
          parallax: false
          position: center
          size: 30%
          text_color_light: true
      spacing:
        padding: ['12%', '0', '0', '0']

  - block: markdown
    content:
      text: '
<div class="home-section">
  <div style="display: flex; gap: 20px; justify-content: center; align-items: center; flex-wrap: wrap;">
    <a href="/research/deep-learning-hardware-design/">
      <div class="image-container">
        <div class="text-overlay">Deep Learning Hardware Design</div>
        <img src="https://github.com/kmuhan/edlo_lab_page/blob/main/content/research/Deep%20Learning%20Hardware%20Design/featured.png?raw=true" alt="Deep Learning Hardware Design">
      </div>
    </a>
    <a href="/research/deep-learning-sw-optimization/">
      <div class="image-container">
        <div class="text-overlay">Deep Learning SW Optimization</div>
        <img src="https://raw.githubusercontent.com/kmuhan/edlo_lab_page/refs/heads/main/content/research/deep-learning-sw-optimization/featured.png" alt="Deep Learning SW Optimization">
      </div>
    </a>
  </div>
</div>

<style>
.home-section {
  padding: 50px 0;
  background: unset;
}

.image-container {
  max-width: 450px; /* 최대 너비 설정 */
  width: 100%; /* 화면 크기에 따라 조정 */
  aspect-ratio: 16 / 10; /* 너비와 높이 비율 유지 */
  overflow: hidden;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  position: relative;
}

.image-container img {
  width: 100%; /* 부모 크기에 맞춤 */
  height: 100%;
  object-fit: cover;
  transition: transform 0.3s ease;
}

.image-container:hover {
  transform: scale(1.05);
  box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
}

.text-overlay {
  position: absolute;
  top: 10px;
  left: 50%;
  transform: translateX(-50%);
  background-color: rgba(0, 0, 0, 0.6);
  color: white;
  padding: 5px 10px;
  border-radius: 5px;
  font-size: 16px;
  font-weight: bold;
  text-align: center;
}

@media screen and (max-width: 768px) {
  .image-container {
    max-width: 300px; /* 작은 화면에서는 크기 축소 */
  }
}

@media screen and (max-width: 480px) {
  .image-container {
    max-width: 100%; /* 모바일에서는 가득 채우기 */
  }
}
</style>


      '
    design:
      columns: '1'
      spacing:
        padding: ['0', '0', '0', '0']
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
      title: Latest Publications
      text: ""
      count: 5
      filters:
        folders:
          - publication
    design:
      view: citation
      columns: '1'
---
