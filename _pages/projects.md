---
layout: page
title: projects
permalink: /projects/
nav: true
nav_order: 2
---

<iframe id="projectsFrame" src="https://nitishnaineni.super.site/projects/" width="100%" frameborder="0"></iframe>

<script>
  // Selecting the iframe element
  var iframe = document.getElementById("projectsFrame");
  
  // Adjusting the iframe height onload event
  iframe.onload = function(){
      iframe.style.height = iframe.contentWindow.document.body.scrollHeight + 'px';
  }
</script>