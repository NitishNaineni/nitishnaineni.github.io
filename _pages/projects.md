---
layout: page
title: projects
permalink: /projects/
nav: true
nav_order: 2
---

<iframe id="projectsFrame" src="https://nitishnaineni.super.site/projects/chess-bot" width="100%" height="1000px"></iframe>

<script>
	let iframe = document.querySelector("#projectsFrame");

	window.addEventListener('message', function(e) {
		// message that was passed from iframe page
		let message = e.data;

		iframe.style.height = message.height + 'px';
	} , false);
</script>