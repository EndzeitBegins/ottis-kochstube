---
layout: page
title: Suche
permalink: /search/
---

<div id="search-container">
    <input type="text" id="search-input" placeholder="Nach Rezepten suchen ...">
    <ul id="results-container"></ul>
</div>

<script src="{{ site.baseurl }}/assets/simple-jekyll-search.min.js" type="text/javascript"></script>

<script>
    SimpleJekyllSearch({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    searchResultTemplate: '<div style="text-align: left !important;"><a href="{url}"><h2 style="text-align:left !important;">{title}</h2></a></div>',
    json: '{{ site.baseurl }}/search.json'
    });
</script>
