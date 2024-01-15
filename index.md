---
share: true
---


this is the index file.

[about](./about.md)

[Welcome](./Welcome.md)

[yet-another-note-to-mom](./LettersToMom/yet-another-note-to-mom.md)

[anoteinsideletterstomom](./LettersToMom/anoteinsideletterstomom.md)


[24-01-14-5-19pm-another test](./LettersToMom/24-01-14-5-19pm-another%20test.md)



Below this is some liquid templating - let's see if it get's published.



{% for page in site.pages %}
	the title is =={{ page.title }}==
	the ID is {{ page.id }}
	 excerpt is{{ page.excerpt }}
	date is {{ page.date | date_to_rfc822 }}
	link is{{site.url}}{{ page.url }}
{% endfor %}    
