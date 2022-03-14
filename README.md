Terminal-based 2048 game implemented in TeX.

### Playing

```
$ (etex|pdftex|xetex|luatex) -translate-file=natural.tcx -cnf-line 'max_print_line=1000' main
```
It is also possible to run the `main.tex` as an executable script. To do this add the line 
```
#!/usr/bin/env -S pdftex -translate-file=natural.tcx -cnf-line 'max_print_line=1000' '\bgroup\let~\expandafter\catcode`#14~\futurelet~~~}\input'
```
to the start of `main.tex`.

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

![Demo](https://github.com/plante3/2048tex/blob/main/demo.gif)
