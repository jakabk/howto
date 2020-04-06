---
#snippet
#python
#ansible
#templating
#include
#jinja2
---

> .path/templates/include.jinja2 is included into .path/templates/template.jinja2
```python
from jinja2 import Environment, FileSystemLoader

file_loader = FileSystemLoader('.path/templates')
environment = Environment(loader = file_loader)

template = environment.get_template('template.jinja2')

variables = {'key': 'value'}
print(template.render(**variables))
```
