.PHONY: all

all: ausarbeitung.pdf

ausarbeitung.pdf: ausarbeitung.tex content/*
	pdflatex -src -interaction=nonstopmode ausarbeitung.tex
	biber ausarbeitung.bcf
	pdflatex -src -interaction=nonstopmode ausarbeitung.tex
	pdflatex -src -interaction=nonstopmode ausarbeitung.tex

clean:
	rm -f *.aux
	rm -f *.bbl
	rm -f *.bcf
	rm -f *.blg
	rm -f *.lof
	rm -f *.log
	rm -f *.out
	rm -f *.run.xml
	rm -f *.toc

realclean: clean
	rm -f *.pdf
