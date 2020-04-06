---
#yaml
#multiline
#pipe
#dash
#right-angle-bracket
#greater-than
#minus
#plus
#ansible
---

# YAML Multiline

[YAML Multiline](yaml-multiline.info)


### ```>``` replace newlines with spaces
> single newline at end
```
replace-newlines: >
··First line\n
··Second line\n
··\n
··Third line\n
··\n
··\n
```
**results**
```
First line Second line\n
Third line\n
```

### ```|``` keep newlines
> single newline at end
```
keep-newlines: |
··First line\n
··Second line\n
··\n
··Third line\n
··\n
··\n
```
**results**
```
First line\n
Second line\n
\n
Third line\n
```

### ```-``` strip new line at end
```
keep-newlines-no-newline-at-end: |-
··First line\n
··Second line\n
··\n
··Third line\n
··\n
··\n
```

**results**
```
First line\n
Second line\n
\n
Third line<no-newline>
```

### ```+``` keep all newlines from end
```
replace-newlines-keep-all-newlines-from-end: >+
··First line\n
··Second line\n
··\n
··Third line\n
··\n
··\n
```
**results**
```
First line\n
Second line\n
\n
Third line\n
\n
\n
```
