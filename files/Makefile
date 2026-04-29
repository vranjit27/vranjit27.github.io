.PHONY: all install clean

all: cv-full.pdf cv-small.pdf

%.pdf: %.tex
	pdflatex -interaction=nonstopmode $<
	pdflatex -interaction=nonstopmode $<

# Copy built PDFs to the filenames the website serves
install: all
	cp cv-full.pdf ranjit_kumaresan_cv.pdf
	cp cv-small.pdf ranjit_kumaresan_cv_short.pdf

clean:
	rm -f *.aux *.log *.out cv-full.pdf cv-small.pdf
