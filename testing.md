---
---

Returns to Scope is an educational project. Our goal is to create tools that help teach economics and policy analysis by making practical, clear, and informative content. 
The name Returns to Scope is the economic theory that you can accomplish more if you dabble a little in many fields, or if you cover a wide array of topics. The goal of this project is to give simple guides to economics and policy in hopes of making teaching tools that spur learning, discussion, and growth. 2

{% for post in site.data.podcast-list %}
	"post : {{ post }}"
	{% for myfile in site.static_files %}
		"myfile : {{ myfile }}"
		{% if myfile.path contains 'podcasts' %}
			<p>{% assign mylocation = myfile.path %} </p>
			<p>{% assign mytime = myfile.modified_time %} </p>
			<p> "1" </p>
			<p>"{{ mylocation }}"</p>
			<p>"{{ mytime }}"</p>
		{% endif %}
	{% endfor %}
{% endfor %}


<!--
**ReturnsToScope/returnstoscope** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
