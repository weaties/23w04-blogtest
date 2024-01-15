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

## collection - 

{{collection}}

itteraring over objects in the collection

	{% for attribute in collection %}
 attribute - {{attribute}} 

{% for subattr in attribute %}
subattr - {{subattr}}
{% endfor %}

{% endfor %}
{% endfor %} 

