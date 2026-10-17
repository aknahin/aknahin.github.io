---
layout: page
title: Publications
description: >
  My work spans design automation, plasmonic devices, and optical sensing.
redirect_from:
  - /publications.html
---

## Peer-reviewed articles

<div class="pubs">
{% for pub in site.data.publications %}
<article class="pub">
  <h3 class="pub-title" tabindex="0">
    {% if pub.url %}<a href="{{ pub.url }}" class="external">{{ pub.title }}</a>{% else %}{{ pub.title }}{% endif %}
  </h3>
  <p class="pub-meta">{{ pub.authors | replace: "Asrafuzzaman Khan Nahin", "<strong>Asrafuzzaman Khan Nahin</strong>" }}<br><em>{{ pub.journal }}</em>, {{ pub.year }}</p>
  <div class="pub-flyout" role="tooltip">
    <dl>
      <dt>Authors</dt><dd>{{ pub.authors }}</dd>
      <dt>Published</dt><dd>{{ pub.date }}</dd>
      <dt>Journal</dt><dd>{{ pub.journal }}{% if pub.volume %}, vol. {{ pub.volume }}{% endif %}{% if pub.pages %}, {{ pub.pages }}{% endif %}</dd>
      <dt>Publisher</dt><dd>{{ pub.publisher }}</dd>
      {% if pub.rank %}<dt>Ranking</dt><dd>{{ pub.rank }}</dd>{% endif %}
      {% if pub.doi %}<dt>DOI</dt><dd><a href="https://doi.org/{{ pub.doi }}" class="external">{{ pub.doi }}</a></dd>{% endif %}
    </dl>
    <p class="pub-abstract">{{ pub.abstract }}</p>
  </div>
</article>
{% endfor %}
</div>

## Manuscript under review

### An Overview of Computer-Aided Printed Circuit Board Routing in the Era of Next-Generation Intelligent Autorouting Techniques
A review of routing methods and the emerging role of intelligent techniques in PCB design automation.  
*Under review.*

## Further reading
Looking for the full record? [Download my CV](/assets/Asrafuzzaman-Khan-Nahin-CV.pdf) for research experience, education, and complete publication details.
