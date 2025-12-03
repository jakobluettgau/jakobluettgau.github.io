SOURCES = $(wildcard *.dot)
OBJECTS_PDF = $(SOURCES:.dot=.pdf)
OBJECTS_PNG = $(SOURCES:.dot=.png)

all: pdf

pdf: $(OBJECTS_PDF) Makefile
png: $(OBJECTS_PNG) Makefile

%.pdf: %.dot
	dot -Tpdf $< -o $@

%.png: %.dot
	dot -Tpng $< -o $@

clean:
	rm $(OBJECTS)
