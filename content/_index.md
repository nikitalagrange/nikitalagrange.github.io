---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing
enableEmoji: true

design:
  # Default section spacin
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume_NL.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: shiny.svg 
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 Research'
      subtitle: ''
      text: |-
        <div style="text-align: left; max-width: 700px; margin: auto; line-height: 1.6;"> 
          <p> I am a PhD student at <a href="https://institut-curie.org/institut-curie-research-center" target="_blank">Institut Curie</a> in Paris. My thesis focuses on causal discovery. More specifically, I am working on extending the <a href="https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005662" target="_blank">MIIC</a> algorithm, developed within <a href="http://kinefold.curie.fr/isambertlab/" target="_blank">the Isambert Lab</a> to a search-and-score mode.
          </p>

          <p>
             The goal is to improve the efficiency and robustness of causal discovery algorithms, 
              particularly when applied to complex and non-linear biomedical data.
          </p>
          <p> Beyond that, I am interested in developing new machine learning algorithms that are more grounded in human reasoning and are interpretable.</p> </div>
    design:
      columns: '1'
  #- block: collection
  #  id: papers
  #  content:
  #    title: Featured Publications
   #   filters:
   #     folders:
   #       - publication
  #      featured_only: true
  #  design:
  #    view: article-grid
  #    columns: 2
  - block: collection
    id: papers
    content:
      title: '📝 Publications'
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
        profile: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Talks
      filters:
        folders:
          - event
    design:
      view: article-grid-summary
      columns: 1

  - block: markdown
    id: services
    content:
      title: Academic Services
      subtitle: ''
      text: |-
        **Representative of doctoral students** on the [EDITE doctoral school board](https://www.edite-de-paris.fr/conseil-de-ledite/)  
        _Participation in the board and involvement in key decision-making processes._

        **Reviewer** for the [NeurIPS BDU Workshop 2024](https://gp-seminar-series.github.io/neurips-2024/)  
        _Reviewed two submissions for the NeurIPS 2024 Workshop on Bayesian Decision-making and Uncertainty._
    columns: '1'

  - block: markdown
    id: news
    content:
      title: "📰 News"
      subtitle: ""
      text: |-
        <style>
          .timeline-wrapper {
            max-width: 750px;
            margin: 3rem auto;
            max-height: 400px;
            overflow-y: auto;
            padding-right: 1rem;
            scroll-behavior: smooth;
          }
          .timeline {
            border-left: 3px solid #ceb2f8;
            padding-left: 1rem;
          }
          .timeline .event {
            position: relative;
            margin-bottom: 2rem;
            padding-left: 1rem;
          }
          .timeline .event::before {
            content: '●';
            color: #ceb2f8;
            position: absolute;
            left: -0.9rem;
            top: 0.15rem;
            font-size: 1.1rem;
          }
          .timeline .date {
            font-weight: bold;
            color: #ceb2f8;
            display: block;
            margin-bottom: 0.2rem;
          }
          .timeline p {
            margin: 0;
            line-height: 1.5;
          }
          .event.hidden {
           opacity: 0;
           max-height: 0;
           overflow: hidden;
           transition: all 0.4s ease;
          }
        #seeMoreBtn {
          display: block;
          margin: 1rem auto;
          background-color: #ceb2f8;
          color: #fff;
          border: none;
          padding: 0.5rem 1rem;
          border-radius: 5px;
          cursor: pointer;
          font-weight: bold;
          }
        #seeMoreBtn:hover {
          background-color: #b290e0;
          }
        </style>

        <div class="timeline-wrapper">
          <section class="timeline">
            <div class="event">
              <span class="date">📅 <strong> January 23, 2025</strong></span>
              <p>Publication of a paper on synthetic health data generation with Institut Roche in <a href="https://www.nature.com/articles/s41746-025-01431-6" target="_blank"><em>npj Digital Medicine</em></a> 🎉 !</p>
            </div>
            <div class="event">
              <span class="date">📅<strong> January 17, 2025</strong></span>
              <p>Publication of a paper on the CausalXtract tool, which extracts features from time series to reconstruct temporal causal networks in <a href="https://elifesciences.org/articles/95485" target="_blank"><i>eLife</i></a> 🎉 !</p>
            </div>
            <div class="event">
              <span class="date">📅<strong> December 23, 2024 </strong></span>
              <p>Publication of the preprint on the extension of the MIIC algorithm to a search-and-score approach applied to categorical data in <a href="https://arxiv.org/abs/2412.17508" target="_blank"><i>arXiv</i></a> 🎉 !</p>
            </div>
            <div class="event hidden">
              <span class="date">📅<strong>October 2024</strong></span>
              <p> Second stay in <a href="https://profiles.imperial.ac.uk/b.bravi21" target="_blank">Dr. Barbara Bravi's</a> team at Imperial College London 🇬🇧</p>
            </div>
            <div class="event hidden">
              <span class="date">📅<strong>September 2024</strong></span>
              <p>Participation in the retreat of young researchers from Institut Curie, Centre des Cordeliers, and Institute of Biotechnology of the Czech Academy of Sciences in Prague 🇨🇿</p>
            </div>
            <div class="event hidden">
              <span class="date">📅<strong>September 2023</strong></span>
              <p>Presentation of my thesis project and preliminary results at the workshop of the <a href="https://centreborelli.ens-paris-saclay.fr/en/artificial-intelligence-data-science-and-cybersecurity" target="_blank">AI-DSCY team</a> at Centre Borelli in Paris 🇫🇷</p>
            </div>
            <div class="event hidden">
              <span class="date">📅<strong>June 2023</strong></span>
              <p>First stay in <a href="https://profiles.imperial.ac.uk/b.bravi21" target="_blank">Dr. Barbara Bravi's</a> team at Imperial College London 🇬🇧</p>
            </div>
            <div class="event hidden">
              <span class="date">📅<strong>October 2022</strong></span>
              <p>Start of my PhD at Institut Curie under the supervision of <a href="http://kinefold.curie.fr/isambertlab" target="_blank">Dr. Hervé Isambert</a> and co-supervised by <a href="https://profiles.imperial.ac.uk/b.bravi21"target="_blank">Dr. Barbara Bravi</a> 🎉 !</p>
            </div>
          </section>
          <button id="seeMoreBtn" onclick="showMoreEvents()">See more</button>
        </div>

        <script>
        function showMoreEvents() {
          const hiddenEvents = document.querySelectorAll('.event.hidden');
          hiddenEvents.forEach(e => e.classList.remove('hidden'));
          document.getElementById('seeMoreBtn').style.display = 'none';
        }
        </script>
    columns: '1'


      # Page type to display. E.g. post, talk, publication...
  - block: markdown
    id: contact
    content:
      title: Contact
      subtitle: ''
      text: |-
        <p style="text-align:center;">
          📧 <a href=mailto:nikita.lagrange@curie.fr>nikita.lagrange@curie.fr</a> or <a href=mailto:nikita.lagrange@tutanota.com>nikita.lagrange@tutanota.com</a><br><br>
          📍Institut Curie, Research Center, CNRS-UMR168 <br>
            Pavillon Curie, 1st floor, Office 01.09.b <br>
            11, rue Pierre et Marie Curie <br> 75005 Paris</p><br>
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1312.8575416863475!2d2.3431009000000063!3d48.844573100000005!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e671c29be381a9%3A0xcebd6da848fd403c!2s11%20Rue%20Pierre%20et%20Marie%20Curie%2C%2075005%20Paris!5e0!3m2!1sfr!2sfr!4v1739726502431!5m2!1sfr!2sfr" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe> 

      columns: '1'


  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

        Easily build anything with blocks - no-code required!
        
        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
