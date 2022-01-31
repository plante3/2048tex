Terminal-based 2048 game implemented in TeX.

### Playing

```
$ (etex|pdftex|xetex|luatex) -translate-file=natural.tcx main
```
It is also possible to run the `main.tex` as an executable script. To do this add the line 
```
#!/usr/bin/env -S pdftex -translate-file=natural.tcx '\bgroup\let~\expandafter\catcode`#14~\futurelet~~~}\input'
```
to the start of `main.tex` and make it executable.

### Controls

movement:
```
     ^
     k
< h     l >  +  ENTER
     j
     v
```

`bye` to quit.

Occationally, there may be display glitches due to the way TeX wraps its output
lines. To fix this, edit your `texmf.cnf` file (you may find it by running
`kpsewhich -a texmf.cnf`, for me it is at `/etc/texmf/web2c/texmf.cnf`) and
add/change the line
```
max_print_line=1000
```

![Demo](https://github.com/plante3/2048tex/blob/main/demo.gif)
