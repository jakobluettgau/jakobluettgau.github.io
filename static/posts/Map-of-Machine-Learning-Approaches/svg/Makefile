SVGFILES := $(wildcard *.svg)

all: pdf


pdf: $(SVGFILES:%.svg=%.pdf)
png: $(SVGFILES:%.svg=%.png)

%.pdf: %.svg
	inkscape -o $*.pdf $*.svg --export-area-page

%.png: %.svg
	inkscape -o $*.png $*.svg --export-area-page 

clean:
	rm -f *.png
	rm -f *.pdf
