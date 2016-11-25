---
layout: page
title: Gallery
subtitle: Eye-candy.
desc: Eye-candy.
permalink: /gallery/
---
<!-- {{ site.baseurl }} -->
{::nomarkdown}
<div>
{% for image in site.static_files %}
    {% if image.path contains 'images/' %}
        <img src="{{ image.path }}" alt="image" />
    {% endif %}
{% endfor %}

</div>
{:/}