---
layout: page
title: projects
permalink: /projects/
nav: true
nav_order: 2
---

<iframe id="projectsFrame" src="https://nitishnaineni.super.site/projects/" width="100%" height="800px" frameborder="0"></iframe>

<script>
document.addEventListener("DOMContentLoaded", function() {
    var currentPath = window.location.pathname;
    var iframePath = currentPath.replace("/projects", "");
    var iframeURL = "https://nitishnaineni.super.site" + iframePath;
    console.log("Setting iframe URL to: " + iframeURL);
    document.getElementById('projectsFrame').src = iframeURL;
});
</script>