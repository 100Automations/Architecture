#### `_automations/`

100 Automations is a website built to host Automations or automatic software programming.
The Automations contain only data inside of the front matter.

There is no markdown contained within the file, and thusly has no content to display.
If you want to display the data within automations you will have to iterate through the data using liquid.

```html
{% for automation in site.automations %}

<h1>
  {{automation.title}}
</h1>

{% endfor %}
```
