# nbconvert-mistune-test
Minimized test case to solve an issue with using mistune 0.7.3 within jupyter nbconvert
To test the conversion, run
``` bash
jupyter-nbconvert --to html html_md_test.ipynb
```
that will produce `html_md_test.html`.
Using 0.7.2 should give the correct result and render the HTML image.
The exact jupyter version does not seem to affect this, 
however, here's my setup:
```
jupyter==1.0.0
jupyter-client==4.3.0
jupyter-console==4.1.1
jupyter-contrib-core==0.3.0
jupyter-core==4.1.0
```

The expected html results in both cases can be seen comparing 
`mistune-0.7.2.html` and `mistune-0.7.3.html`.
