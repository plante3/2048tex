Terminal-based 2048 game implemented in TeX.

### Building

```
$ (tex|pdftex|xetex|luatex) -shell-escape main
```

`-shell-escape` is needed for escape codes.

### Controls

movement:
```
     ^
     k
< h     l >  +  ENTER
     j
     v

```

`bye` or `^D` to quit.

![Demo](https://github.com/plante3/2048tex/main/demo.gif)