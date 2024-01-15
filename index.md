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



# page titles
{% for page in site.pages %}

[{{ page.title }}]({{site.url}}{{ page.url }})

{% endfor %}    


# collections

{% for collection in site.collections %}

## collection - {{collection}}

	{% for page in collection %}

### page - {{page.title}} -> {{page.url}}

{% endfor %}
{% endfor %} 