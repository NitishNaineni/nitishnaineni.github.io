---
layout: page
title: projects
permalink: /projects/
description: A growing collection of your cool projects.
nav: true
nav_order: 2
---

<iframe id="projectsFrame" src="https://nitishnaineni.super.site/projects/" width="100%" height="800px" frameborder="0"></iframe>

<script>
document.getElementById('projectsFrame').addEventListener('load', function() {
    var iframeURL = this.contentWindow.location.href;
    updateBrowserURL(iframeURL);
});

function updateBrowserURL(iframeURL) {
    var newURL = iframeURL.replace("https://nitishnaineni.super.site", "{{ site.baseurl }}");
    window.history.pushState({}, "", newURL);
}

var currentURL = window.location.href;
if (currentURL.includes("{{ site.baseurl }}/projects/")) {
    var iframeURL = currentURL.replace("{{ site.baseurl }}", "https://nitishnaineni.super.site");
    document.getElementById('projectsFrame').src = iframeURL;
}
</script>