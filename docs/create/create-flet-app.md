---
title: Create Flet app
---

To create a new "minimal" Flet app run the following command:

```
flet create <project-name>
```

for example:

```
flet create my_flet_app
```

`<project-name>` will be used as a name of output directory.

Flet will create `<project-name>` directory with the following `main.py`:

```python
import flet as ft

def main(page: ft.Page):
    page.add(ft.SafeArea(ft.Text("Hello, Flet!")))

ft.app(main)
```

Flet program has `main()` function where you would add UI elements ([controls](flet-controls)) to a page or a window. The application ends with a blocking `ft.app()` function which initializes Flet app and [runs](running-app) `main()`.

To create a new Flet app from "counter" template run the following command:

```
flet create --template counter <project-name>
```

Async or not async?

Creating async from template, limnk to other doc