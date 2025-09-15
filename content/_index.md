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
        url: uploads/CV_NL.pdf
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
          <p> Beyond that, I am interested in developing machine learning algorithms that are more grounded in human reasoning and are interpretable.</p> </div>
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
            margin: 1rem auto;
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
          .toggle-btn {
          display: block;
          margin: 1rem auto;
          background-color: #6b3fa0;
          color: #ffffff;
          border: none;
          padding: 0.5rem 1rem;
          border-radius: 5px;
          cursor: pointer;
          font-weight: bold;
          transition: background-color 0.3s ease, transform 0.2s ease;
        }
        .toggle-btn:hover {
          background-color: #582f89;
          transform: translateY(-2px);
        }        
        </style>


        <div class="timeline-wrapper">
          <section class="timeline">
           <div class="event">
            <span class="date">📅 <strong>September 1-5, 2025</strong></span>
              <p>I had the pleasure of attending the <a href="https://paiss.inria.fr/" target="_blank">PRAIRIE/MIAI Artificial Intelligence Summer School (P.A.I.S.S.) </a> in Grenoble 🇫🇷 . It was an unforgettable week of world-class talks from Yann LeCun to Michael Jordan and a community that made the learning stick. I met passionate students from around the world 🌍 and learned a lot through discussions and poster sessions. </br>
                My gratitude 🙏 goes to the organizers, volunteers and sponsors.</p>
           </div>
           <div class="event">
            <span class="date">📅 <strong>July 21-26, 2025</strong></span>
              <p>I had the pleasure of attending the <a href="https://www.eeml.eu/" target="_blank">Eastern European Machine Learning (EEML) Summer School </a> in Sarajevo 🇧🇦, a vibrant event that brought together participants from 44 countries, with over half representing Eastern Europe. This diversity is a key strength of science and collaboration. </br>
                My warmest thanks 🙏 to the amazing organizing team, volunteers, lecturers, and sponsors who made this event possible and accessible.</p>
          </div>
          <div class="event">
            <span class="date">📅 <strong>May 1, 2025</strong></span>
              <p>Our method for search-and-score learning of ancestral graphs has been accepted at <a href="https://openreview.net/forum?id=RfqTvlo9XQ" target="_blank">ICML 2025</a> in Vancouver 🇨🇦 ! Looking forward to presenting this work 🎉 !</p>
          </div>
            <div class="event">
              <span class="date">📅 <strong>March 11, 2025</strong></span>
                <p>I presented my PhD thesis in 3 minutes during the EDITE 2025 Doctoral Day at the Centre Pompidou in Paris 🇫🇷 . An exciting challenge in science communication 📣 !</p>
            </div>
            <div class="event hidden">
              <span class="date">📅 <strong>February 21, 2025</strong></span>
                <p>Our contribution on a feedback from a new hybrid learning approach has been accepted at <a href="https://www.conftool.com/qpes2025/index.php?page=browseSessions&cols=3&form_session=30&mode=table" target="_blank">QPES2025</a> in Brest 🇫🇷 🎉 ! This work results from a data analysis consulting mission at <a href="https://capsule.sorbonne-universite.fr/" target="_blank">CAPSULE</a>, Sorbonne University 🎓</p>
            </div>
            <div class="event hidden">
              <span class="date">📅 <strong> January 23, 2025</strong></span>
              <p>Publication of a paper on synthetic health data generation with Institut Roche in <a href="https://www.nature.com/articles/s41746-025-01431-6" target="_blank"><em>npj Digital Medicine</em></a> 🎉 !</p>
            </div>
            <div class="event hidden">
              <span class="date">📅<strong> January 17, 2025</strong></span>
              <p>Publication of a paper on the CausalXtract tool, which extracts features from time series to reconstruct temporal causal networks in <a href="https://elifesciences.org/articles/95485" target="_blank"><i>eLife</i></a> 🎉 !</p>
            </div>
            <div class="event hidden">
              <span class="date">📅<strong> December 23, 2024 </strong></span>
              <p>Publication of the preprint on the extension of the MIIC algorithm to a search-and-score approach applied to categorical data in <a href="https://arxiv.org/abs/2412.17508" target="_blank"><i>arXiv</i></a> 🎉 !</p>
            </div>
            <div class="event hidden">
              <span class="date">📅<strong> October 2024</strong></span>
              <p> Second stay in <a href="https://profiles.imperial.ac.uk/b.bravi21" target="_blank">Dr. Barbara Bravi's</a> team at Imperial College London 🇬🇧</p>
            </div>
            <div class="event hidden">
              <span class="date">📅<strong> September 2024</strong></span>
              <p>Participation in the retreat of young researchers from Institut Curie, Centre des Cordeliers, and Institute of Biotechnology of the Czech Academy of Sciences in Prague 🇨🇿</p>
            </div>
            <div class="event hidden">
              <span class="date">📅<strong> September 2023</strong></span>
              <p>Presentation of my thesis project and preliminary results at the workshop of the <a href="https://centreborelli.ens-paris-saclay.fr/en/artificial-intelligence-data-science-and-cybersecurity" target="_blank">AI-DSCY team</a> at Centre Borelli in Paris 🇫🇷</p>
            </div>
            <div class="event hidden">
              <span class="date">📅<strong> June 2023</strong></span>
              <p>First stay in <a href="https://profiles.imperial.ac.uk/b.bravi21" target="_blank">Dr. Barbara Bravi's</a> team at Imperial College London 🇬🇧</p>
            </div>
            <div class="event hidden">
              <span class="date">📅<strong> October 2022</strong></span>
              <p>Start of my PhD at Institut Curie under the supervision of <a href="http://kinefold.curie.fr/isambertlab" target="_blank">Dr. Hervé Isambert</a> and co-supervised by <a href="https://profiles.imperial.ac.uk/b.bravi21"target="_blank">Dr. Barbara Bravi</a> 🎉 !</p>
            </div>
          </section>
            <button id="toggleBtn" class="toggle-btn" onclick="toggleEvents()">See more</button>
          </div>

        <script>
        function toggleEvents() {
        const hiddenEvents = document.querySelectorAll('.event.hidden');
        const toggleBtn = document.getElementById('toggleBtn');
        const isHidden = hiddenEvents.length > 0;

        if (isHidden) {
          hiddenEvents.forEach(e => e.classList.remove('hidden'));
          toggleBtn.textContent = 'See less';
        } else {
          const allEvents = document.querySelectorAll('.event');
          allEvents.forEach((e, index) => {
            if (index >= 3) e.classList.add('hidden');
          });
          toggleBtn.textContent = 'See more';
          }
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
          📧 <a href=mailto:nikita.lagrange@curie.fr>nikita.lagrange@curie.fr</a> or <a href=mailto:lagrangenikita@gmail.com>lagrangenikita@gmail.com</a><br><br>
          📍Institut Curie, Research Center, CNRS-UMR168 <br>
            Pavillon Curie, 1st floor, Office 01.09.b <br>
            11, rue Pierre et Marie Curie <br> 75005 Paris</p><br>

          <div style="margin-top: 20px; border: 1px solid #444; border-radius: 8px; overflow: hidden; box-shadow: 0 2px 5px rgba(0,0,0,0.3);">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1312.8575416863475!2d2.3431009000000063!3d48.844573100000005!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e671c29be381a9%3A0xcebd6da848fd403c!2s11%20Rue%20Pierre%20et%20Marie%20Curie%2C%2075005%20Paris!5e0!3m2!1sfr!2sfr!4v1739726502431!5m2!1sfr!2sfr"
              width="100%" height="400" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade">
            </iframe>
          </div>
        </div>  
      
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
