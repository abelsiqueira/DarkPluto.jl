# Dark Pluto

A hack to have custom CSS on Pluto.

Currently this is just the instructions and my custom CSS.

## Instructions

1. To avoid clashes, clone `Pluto`:
```
git clone https://github.com/fonsp/Pluto.jl
```

2. Now, place `pluto-custom.css` inside `.../Pluto.jl/frontend/`.

3. Now, edit `.../frontend/editor.html` and add
```
<link rel="preload" href="./pluto-config.css" as="style">
```

4. Now, edit `.../frontend/index.css` and add
```
@import url("pluto-custom.css");
```

5. Now, edit `.../frontend/treeview.css` and add
```
@import url("pluto-custom.css");
```