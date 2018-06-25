---
title: MAMP & MAMP PRO Documentation > Search
description: MAMP & MAMP PRO Documentation Search
layout: default-1
language: en
---

## Search

<div id="tipue_search_content"></div>

<script>
var tipuesearch = {"pages": [
  {% for page in site.pages %}
    {% if page.url contains "/en/" %}
      {% if page.url contains "/en/Search/" %}
          
      {% else %}
        {% if page.url contains "windows" %}
          
        {% else %}
          {"title": "{{page.title | replace_first: ' Documentation', ''}}", "text": "{{page.content | remove: '\' | markdownify | strip_html | strip_newlines | xml_escape}}", "tags": "", "url": "{{page.url}}"},
        {% endif %}
      {% endif %}
    {% endif %}
  {% endfor %}
  {"title": "", "text": "", "tags": "", "url": ""}
]};

var tipuesearch_string_5 = 'Results';

$(document).ready(function() {
  $('#tipue_search_input').tipuesearch({
    'mode': 'static',
    'show': 100,
    'showTitleCount': false,
    'minimumLength': 1
  });
});
</script>
