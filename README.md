# spritely
Create an svg sprite file from other svg files

# Installation
```bash
pipx install spritely
```

# Usage
```bash
spritely --config {path to config file} > /tmp/my-new-sprite-file.svg
```

Then, in insert the sprite into your document:

```xml
<svg><use> xlinkHref="my-new-sprite-file.svg#___icon-name___"</use></svg>
```
where `___icon-name___` is the name of one of the icons in the config file.

# Configuration
```yaml
---
root_path: /home/marbex7/{path-to-svg-files}
sources:
  - file_name: ic.svg
    icon_name: "my-ic-icon"
  - file_name: a.svg
    icon_name: "my-a-icon"
  - file_name: t.svg
    icon_name: "my-t-icon"
  - file_name: sprite_test.svg
    icon_name: "my-sprite-test-icon"
  - file_name: g.svg
    icon_name: "my-g-icon"
  - file_name: xw.svg
    icon_name: "my-xw-icon"
  - file_name: x.svg
    icon_name: "my-x-icon"
...
```
