---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: TinyMagic 🔮
---

<div id="home">
  <p>Hi, I'm Rich, by day I'm a <a href="https://www.linkedin.com/in/richpublic" target="_blank" rel="noopener noreferrer">Product Manager</a> at <a href="https://www.zendesk.com" target="_blank" rel="noopener noreferrer">Zendesk</a> helping to build out our beautifully simple enterprise platform. By night I work at building some of the ideas on my almost endless list of cool tiny products.</p> 
  <br>
  <p>This website will be used to capture the journey. Check out my Product page for progress</p>

  <div class="columns">
    <div class="column">
      <h3>🪄Tiny Products</h3>
      <ul>
        {% for project in site.data.projects %}
        <li>
          <a href="{{ project.url }}">{{ project.name }}</a>
        </li>
        {% endfor %}
      </ul>
    </div>

    <div class="column">
      <h3>📒Blog</h3>
      <p>Check out my <a href="/blog">tiny blog</a> for the latest updates.</p>
    </div>

    <div class="column">
      <h3>🔭Find Me</h3>
      <ul>
        <li><a href="https://twitter.com/rich_low" target="_blank" rel="noopener noreferrer">Twitter</a></li>
        <li><a href="https://github.com/richlow" target="_blank" rel="noopener noreferrer">GitHub</a></li>
        <li><a href="https://www.linkedin.com/in/richpublic" target="_blank" rel="noopener noreferrer">LinkedIn</a></li>
        <!-- Add more as needed -->
      </ul>
    </div>

  </div>
  Get product updates:
  <script async src="https://eomail6.com/form/7882d194-fa87-11ed-a741-ad771fd0071d.js" data-form="7882d194-fa87-11ed-a741-ad771fd0071d"></script>
</div>
