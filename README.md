# Dark Pluto

A hack to have custom CSS on Pluto.

Currently this is just the instructions and my custom CSS.

## Instructions

1. To avoid clashes, dev `Pluto`:
```
pkg> dev Pluto
```
This should create `~/.julia/dev/Pluto/`, which is the root of the other files below:

2. Now, place `pluto-custom.css` inside `.../Pluto/frontend/`.

3. Now, edit `.../frontend/editor.html` and add
```
<link rel="preload" href="./pluto-custom.css" as="style">
```
after similar commands.

4. Now, edit `.../frontend/index.css` and add
```
@import url("pluto-custom.css");
```
after similar commands.

5. Now, edit `.../frontend/treeview.css` and add
```
@import url("pluto-custom.css");
```
after similar commands.

