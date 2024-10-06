.PHONY: all clean run

export TEXINPUTS := .:${PWD}/../Commons//:${TEXINPUTS}

all: main.pdf

%.pdf: %.tex
	pdflatex $<

clean:
	rm -f main.aux main.log main.nav main.out main.pdf main.snm main.toc texput.log

run: main.pdf
	xdg-open $<
