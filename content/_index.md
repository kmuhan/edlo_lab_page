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
<div style="display: flex; gap: 20px; justify-content: center; align-items: center;">
  <a href="/research/deep-learning-hardware-design/">
    <div class="image-container" style="position: relative;">
      <div class="text-overlay">Deep Learning Hardware Design</div>
      <img src="https://github.com/kmuhan/edlo_lab_page/blob/main/content/research/Deep%20Learning%20Hardware%20Design/featured.png?raw=true" style="width: 100%; height: 100%; object-fit: cover;">
    </div>
  </a>
  <a href="/research/deep-learning-sw-optimization/">
    <div class="image-container" style="position: relative;">
      <div class="text-overlay">Deep Learning SW Optimization</div>
      <img src="https://raw.githubusercontent.com/kmuhan/edlo_lab_page/refs/heads/main/content/research/deep-learning-sw-optimization/featured.png" style="width: 100%; height: 100%; object-fit: cover;">
    </div>
  </a>
</div>

<style>
.home-section {
    padding: 50px 0;
}

.image-container {
  width: 400px;
  height: 250px;
  overflow: hidden;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* 기본 box shadow */
  transition: transform 0.3s ease, box-shadow 0.3s ease; /* 부드러운 전환 효과 */
  position: relative; /* 텍스트를 절대 위치로 설정하기 위해 필요 */
}

.image-container img {
  object-fit: cover;
  transition: transform 0.3s ease; /* 이미지 확대 전환 효과 */
}

/* 호버링 효과 */
.image-container:hover {
  transform: scale(1.05); /* 컨테이너 크기를 약간 확대 */
  box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2); /* 강조된 shadow */
}

/* 텍스트 스타일 */
.text-overlay {
  position: absolute;
  top: 10px; /* 텍스트의 위쪽 위치 */
  left: 50%; /* 텍스트를 중앙 정렬 */
  transform: translateX(-50%); /* 정확한 중앙 정렬 */
  background-color: rgba(0, 0, 0, 0.6); /* 반투명 배경 */
  color: white; /* 텍스트 색상 */
  padding: 5px 10px; /* 텍스트 주변 간격 */
  border-radius: 5px; /* 약간 둥근 모서리 */
  font-size: 16px; /* 텍스트 크기 */
  font-weight: bold; /* 텍스트 굵기 */
  text-align: center;
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
