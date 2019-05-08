
Available online thanks to github pages: https://stfl.github.io/docker_paper/slides.html

generate PDF with pandoc Latex

~~~
pandoc  --to="latex" --output="docker_new.pdf" --filter="pandoc-crossref" --pdf-engine="xelatex" --bibliography="references.bib" "docker_new.pdc"
~~~

or with vim-pandoc

~~~
:Pandoc! pdf --filter pandoc-crossref
~~~

generate reveal.js slides

~~~
pandoc --to=revealjs --standalone --output=slides.html slides.pdc -V revealjs-url=./reveal.js -V theme=moon --css slides.css
~~~
