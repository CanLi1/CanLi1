---
title: "Li Group - Publications"
layout: gridlay
excerpt: "Li Group -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

## Group highlights

(For a full list see [below](#full-list) or go to <a href="https://scholar.google.com/citations?user=EkwNNlAAAAAJ&hl=en" target="_blank">Google Scholar</a>, <a href="https://www.researchgate.net/profile/Can-Li-9" target="_blank">ResearchGate</a>.

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="95%" style="display:block; margin-left: auto; margin-right: auto;" />
  <p>{{ publi.description }}</p>
  <p>{{ publi.authors }}</p>
  <p><strong><em>{{ publi.journal }}{{ publi.year }}</em></strong></p>
  <p> 
    {% if publi.paper != null %}<a class="btn btn-outline-primary my-1 mr-1 btn-sm" href="{{publi.paper}}" target="_blank" rel="noopener">Paper</a>{% else %}<a></a>{% endif %}
   {% if publi.preprint != null %}<a class="btn btn-outline-primary my-1 mr-1 btn-sm" href="/images/preprint/{{ publi.preprint }}"  target="_blank" rel="noopener">Preprint</a>{% else %}<a></a>{% endif %}
    {% if publi.bibtex != null %}<a class="btn btn-outline-primary my-1 mr-1 btn-sm" href="/images/bibtex/{{ publi.bibtex }}"  target="_blank" rel="noopener">Bibtex</a>{% else %}<a></a>{% endif %}
    {% if publi.slides != null %}<a class="btn btn-outline-primary my-1 mr-1 btn-sm" href="/images/slides/{{ publi.slides }}"  target="_blank" rel="noopener">Slides</a>{% else %}<a></a>{% endif %}
  </p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Full List

{% for publi in site.data.publist %}

  {{ publi.title }}<br/>
  {{ publi.authors }}<br/>
  <strong><em>{{ publi.journal }}{{ publi.year }}</em></strong>
    {% if publi.paper != null %}<a class="btn btn-outline-primary my-1 mr-1 btn-sm" href="{{publi.paper}}" target="_blank" rel="noopener">Paper</a>{% else %}<a></a>{% endif %}
   {% if publi.preprint != null %}<a class="btn btn-outline-primary my-1 mr-1 btn-sm" href="/images/preprint/{{ publi.preprint }}"  target="_blank" rel="noopener">Preprint</a>{% else %}<a></a>{% endif %}
    {% if publi.bibtex != null %}<a class="btn btn-outline-primary my-1 mr-1 btn-sm" href="/images/bibtex/{{ publi.bibtex }}"  target="_blank" rel="noopener">Bibtex</a>{% else %}<a></a>{% endif %}
    {% if publi.slides != null %}<a class="btn btn-outline-primary my-1 mr-1 btn-sm" href="/images/slides/{{ publi.slides }}"  target="_blank" rel="noopener">Slides</a>{% else %}<a></a>{% endif %}
    <br/>
   

{% endfor %}
