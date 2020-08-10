Pico Yet Another Linker Plugin
==============================

This Pico plugin adds the ability to create links with less typing in Markdown.

Install
-------

1. Clone this Github repo into your `plugins/PicoYalinker` directory.
2. If you want to include UTF-8 characters in slugs, add the following line to `config/config.yml`:
   ```
   yalinker_utf8_slugs: true
   ```

Usage
-----

| YALink | Markdown |
| ------ | -------- |
| `[[Page Title]]` | `[Page Title](page-title)` |
| `[[Page Title\|Link Text]]` | `[Link Text](page-title)` |
| `[[Slashes//in Page Title]]` | `[Slashes/in Page Title](slashes-in-page-title)` |
| `[[../Some Path/Page Title]]` | `[Page Title](../some-path/page-title)` |
| `[[../Some Path/Page Title\|]]` | `[../Some Path/Page Title](../some-path/page-title)` |
| `[[/Root Path/Page Title]]` | `[Page Title](/root-path/page-title)` |
| `[[https://example.com]]` | `<https://example.com>` |
| `[[mailto:me@example.com]]` | `<mailto:me@example.com>` |
| `[[mail:me@example.com]]` | `[me@example.com](mailto:me@example.com)` |

Demo
----

https://demo.isnew.info/pico/pico-yalinker

Credits
-------

Author: Huidae Cho
