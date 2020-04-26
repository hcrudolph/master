CC=pdflatex
ACC=makeglossaries
BCC=biber
SOURCES=document
TEX_SOURCES=$(SOURCES:=.tex)

all: pdf1 bib pdf2

nobib: pdf1 glo pdf2

pdf1 pdf2 pdf3: document.tex
	$(CC) $(TEX_SOURCES)

bib: document.tex
	$(BCC) $(SOURCES)

glo: document.tex
	$(ACC) $(SOURCES)

clean:
	rm -f document.pdf *.alg *.acr *.glo *.gls *.glg *.xml *.ist *.lof *.log *.acn *.bbl *.out *.lot *.blg *.aux *.bcf *.dvi *.idx *.toc *.toa *.loappfigure
