INFILES := $(wildcard *.pdf)

all: png

png: $(INFILES:%.pdf=%.png)

%.png: %.pdf
	pdftoppm $*.pdf $* -png

clean:
	rm -f *.png
