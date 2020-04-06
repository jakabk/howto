---
#python
#snippet
#argparse
#standard-library
#optional
#boolean
#default
---

[The add_argument() method](https://docs.python.org/3/library/argparse.html#argparse.ArgumentParser.add_argument)

```python
import argparse

parser = argparse.ArgumentParser()
parser.add_argument(
    '-o', '--optional',
    action = 'store_true',
    default = False
)

args = parser.parse_args([])
print('Called without arguments:', args.optional)

args = parser.parse_args(['--optional'])
print('Called with --optional:', args.optional)
```
