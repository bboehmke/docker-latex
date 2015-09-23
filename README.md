LaTeX environment
=================

Usage
-----

If you have an latex document "Document.tex" in the actual directory you can 
build the PDF with:

```
docker run --rm -it \
    --user="$(id -u):$(id -g)" \
    -v $PWD:/data \
    bboehmke/latex \
    pdflatex Document.tex
```
