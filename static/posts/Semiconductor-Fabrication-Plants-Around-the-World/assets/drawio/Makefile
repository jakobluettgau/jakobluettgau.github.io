DRAWIO_FILES := $(wildcard *.drawio)

all: pdf


pdf: $(DRAWIO_FILES:%.drawio=%.pdf)
png: $(DRAWIO_FILES:%.drawio=%.png)

%.pdf: %.drawio
	drawio -x -f pdf -o $*.pdf $*.drawio --crop

%.png: %.drawio
	drawio -x -f pdf -o $*.png $*.drawio

clean:
	rm -f *.png
	rm -f *.pdf
