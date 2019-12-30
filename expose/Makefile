CC=pdflatex
ACC=makeglossaries
BCC=biber
SOURCES=main
TEX_SOURCES=$(SOURCES:=.tex)

all: pdf1 bib pdf2

nobib: pdf1 glo pdf2

pdf1 pdf2 pdf3: main.tex
	$(CC) $(TEX_SOURCES)

bib: main.tex
	$(BCC) $(SOURCES)

glo: main.tex
	$(ACC) $(SOURCES)

clean:
	rm -f document.pdf *.alg *.acr *.glo *.gls *.glg *.xml *.ist *.lof *.log *.acn *.bbl *.out *.lot *.blg *.aux *.bcf *.dvi *.idx *.toc *.toa *.loappfigure
