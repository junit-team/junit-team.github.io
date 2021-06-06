# JUnit Website

## Generating redirects to former JUnit 4 pages

```sh
gfind . -regex '.*.html' > ~/Desktop/FILES
while read i ; do mkdir -p "$(dirname "$i")"; done < ~/Desktop/FILES
while read i ; do cat license.html > $i; done < ~/Desktop/FILES
```
