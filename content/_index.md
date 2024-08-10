---
# Leave the homepage title empty to use the site title
title: ""
date: 2024-08-09
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      # button:
      #   text: Download CV
      #   url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: sun-tornado-2.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: collection
    content:
      title: Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation

  - block: markdown
    content:
      title: 'My Baby Cat -- JuanJuan'
      subtitle: ''
      text: |-
       <img src="/static/images/1.jpeg" alt="Image 1">
<style>
        .carousel-container {
          max-width: 300px;
          position: relative;
          margin: auto;
          overflow: hidden;
        }
        .carousel-slides {
          display: flex;
          transition: transform 0.5s ease-in-out;
        }
        .carousel-slides img {
          width: 300px;
          height: auto;
          flex-shrink: 0;
        }
        .prev, .next {
          cursor: pointer;
          position: absolute;
          top: 50%;
          width: auto;
          padding: 16px;
          margin-top: -22px;
          color: white;
          font-weight: bold;
          font-size: 18px;
          transition: 0.6s ease;
          border-radius: 0 3px 3px 0;
          user-select: none;
        }
        .next {
          right: 0;
          border-radius: 3px 0 0 3px;
        }
        .prev {
          left: 0;
        }
        </style>
        <div class="carousel-container">
          <div class="carousel-slides">
            <img src="/static/images/1.jpeg" alt="Image 1">
            <img src="/static/images/2.jpeg" alt="Image 2">
            <img src="/static/images/3.jpeg" alt="Image 3">
            <img src="/static/images/4.jpeg" alt="Image 4">
            <img src="/static/images/5.jpeg" alt="Image 5">
            <img src="/static/images/6.jpeg" alt="Image 6">
            <img src="/static/images/7.jpeg" alt="Image 7">
            # <img src="/images/8.jpeg" alt="Image 8">
            # <img src="/images/9.jpeg" alt="Image 9">
          </div>
          <a class="prev" onclick="moveSlides(-1)">&#10094;</a>
          <a class="next" onclick="moveSlides(1)">&#10095;</a>
        </div>

        <script>
        let currentIndex = 0;

        function moveSlides(n) {
          const slides = document.querySelector('.carousel-slides');
          const totalSlides = slides.children.length;
          currentIndex = (currentIndex + n + totalSlides) % totalSlides;
          slides.style.transform = `translateX(-${currentIndex * 300}px)`;
        }
        </script> 2JuanJuan is a charming young Ragdoll cat, born on March 12, 2023. He’s an exceptionally well-behaved and gentle boy, who loves nothing more than rubbing against people and indulging in a soothing massage. JuanJuan has a playful spirit, especially when it comes to interacting with birds, which he finds endlessly entertaining. He also enjoys basking in the sun, soaking up its warmth with contentment. He loves staying by my side while I work, making him the perfect, affectionate companion. 
    design:
      columns: '1'
  # - block: collection
  #   id: papers
  #   content:
  #     title: Featured Publications
  #     filters:
  #       folders:
  #         - publication
  #       featured_only: true
  #   design:
  #     view: article-grid
  #     columns: 2

  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent Academic Presentations
  #     filters:
  #       folders:
  #         - talks
  #   design:
  #     view: article-grid
  #     columns: 1
  # - block: collection
  #   id: news
  #   content:
  #     title: Recent News
  #     subtitle: ''
  #     text: ''
  #     # Page type to display. E.g. post, talk, publication...
  #     page_type: post
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     view: date-title-summary
  #     # Reduce spacing
  #     spacing:
  #       padding: [0, 0, 0, 0]
  # - block: cta-card
  #   demo: true # Only display this section in the Hugo Blox Builder demo site
  #   content:
  #     title: 👉 Build your own academic website like this
  #     text: |-
  #       This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

  #       <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

  #       Easily build anything with blocks - no-code required!
        
  #       From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
  #     button:
  #       text: Get Started
  #       url: https://hugoblox.com/templates/
  #   design:
  #     card:
  #       # Card background color (CSS class)
  #       css_class: "bg-primary-700"
  #       css_style: ""
---
