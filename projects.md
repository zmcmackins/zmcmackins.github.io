---
title: Projects
layout: main
---

<p>Projects</p>
{%for project in site.projects%}
<article>
	<h2>
	<a href="{{site.baseurl}}{project.url}}">{{project.title}}</a>
	</h2>
	<p>
	{{project.excerpt}}
	</p>
	<p><a href="{{site.baseurl}}{{project.url}}">Continue Reading...</a></p>
</article>
{%endfor%}
