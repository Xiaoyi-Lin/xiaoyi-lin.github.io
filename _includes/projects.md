<h2 id="publications">Researchs</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.projects.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 pic" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% endif %}
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ link.page }}">{{ link.title }}</a></div>
      <div class="periodical"><em>{{ link.affiliation }}</em></div>
      <div class="author">{{ link.description }}</div>
  </div>
</div>
</li>

<br>

{% endfor %}

</ol>
</div>