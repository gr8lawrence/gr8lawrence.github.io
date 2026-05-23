---
---

<div class="home-sidebar">

  <aside class="sidebar-panel">
    <img
      src="{{ 'images/tianyi_headshot.jpg' | relative_url }}"
      class="sidebar-photo"
      alt="Tianyi Liu"
      loading="lazy"
    >
    <div class="sidebar-panel-info">
      <p class="sidebar-name">Tianyi Liu</p>
      <p class="sidebar-role">Clinical Biostatistician<br>&amp; Data Scientist</p>
      <p class="sidebar-affiliation">Ph.D. Biostatistics<br>UNC Chapel Hill, 2024</p>
    </div>
    <div class="sidebar-links">
      <a href="https://github.com/gr8lawrence" target="_blank" rel="noopener noreferrer" aria-label="GitHub">
        <i class="fa-brands fa-github"></i> GitHub
      </a>
      <a href="https://www.linkedin.com/in/tianyi-liu-157874133" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn">
        <i class="fa-brands fa-linkedin"></i> LinkedIn
      </a>
      <a href="https://orcid.org/0000-0002-2484-2478" target="_blank" rel="noopener noreferrer" aria-label="ORCID">
        <i class="fa-brands fa-orcid"></i> ORCID
      </a>
      <a href="https://scholar.google.com/citations?user=rgq62U4AAAAJ" target="_blank" rel="noopener noreferrer" aria-label="Google Scholar">
        <i class="fa-brands fa-google"></i> Scholar
      </a>
    </div>
    <a class="button sidebar-cta" href="{{ 'members/tianyi-liu.html' | relative_url }}">Full Bio &amp; CV</a>
  </aside>

  <div class="sidebar-main">

    <h2>About Me</h2>

    <p>
      Hi! Nice to meet you. I am a clinical biostatistician/data scientist. I obtained a
      Ph.D. in <a href="https://sph.unc.edu/bios/biostatistics/">Biostatistics</a> at The
      University of North Carolina at Chapel Hill in August 2024. My research focused on
      <a href="https://en.wikipedia.org/wiki/Cellular_deconvolution">cell type deconvolution</a>
      but also branched out into
      <a href="https://en.wikipedia.org/wiki/Personalized_medicine">precision medicine</a>.
      During my Ph.D. program, I collaborated with a diverse group of experts to tackle
      real-world problems in public health and allied health sciences. I currently work for a
      pharmaceutical company near Philadelphia.
    </p>

    <p>
      In my spare time, I love to read good books, travel to new places, savor delicious meals,
      stay active with sports, and join trivia games. I also maintain a keen interest in playing
      Texas Hold'em and other poker variations. Of course, nothing beats spending quality time
      with my friends and hanging with my cat <a href="{{ 'members/wrigley.html' | relative_url }}">Wrigley</a>.
    </p>

    <p>
      Besides this website, I also maintain a non-technical blog called
      <a href="https://gr8lawrence.com/" target="_blank" rel="noopener noreferrer">A Statistician's Journey</a>.
      Tune in if you would like to see more personal reflections and life updates from me.
    </p>

    <h2>Recent Publications</h2>

    {% assign recent_citations = site.data.citations | sort: "date" | reverse | slice: 0, 3 %}
    {% for cite in recent_citations %}
    <div class="pub-item">
      <div class="pub-title">
        <a href="{{ cite.link }}" target="_blank" rel="noopener noreferrer">{{ cite.title }}</a>
      </div>
      <div class="pub-meta">
        {% assign authors = cite.authors %}
        {% if authors.size > 3 %}
          {{ authors[0] }}, {{ authors[1] }}, {{ authors[2] }} et al.
        {% else %}
          {{ authors | join: ", " }}
        {% endif %}
        &nbsp;&middot;&nbsp;
        <em>{{ cite.publisher }}</em>
        &nbsp;&middot;&nbsp;
        {{ cite.date | date: "%Y" }}
      </div>
    </div>
    {% endfor %}

    <a class="sidebar-see-all" href="{{ 'research/' | relative_url }}">See all publications &rarr;</a>

    <h2>Featured Projects</h2>

    {% for project in site.data.projects %}
      {% if project.group == "featured" %}
      <div class="pub-item">
        <div class="pub-title">
          <a href="{{ project.link }}" target="_blank" rel="noopener noreferrer">{{ project.title }}</a>
        </div>
        <div class="pub-meta">{{ project.subtitle }}</div>
      </div>
      {% endif %}
    {% endfor %}

    <a class="sidebar-see-all" href="{{ 'projects/' | relative_url }}">See all projects &rarr;</a>

  </div>

</div>
