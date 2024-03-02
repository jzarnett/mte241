SLIDES != ./slides.sh
CREATE_DEPS != ./createMakefileDependencies.sh

.PHONY: all clean
all: $(SLIDES) 

include makefileDependencies/*.d

clean:
	rm -f *~ *.aux *.log *.bbl *.blg *.brf *.cb *.ind *.idx *.ilg *.pdfsync *.xdv  \
		*.inx *.ps *.dvi *.toc *.out *.nav *.snm *.d *.bak _region* *.vrb *.fls *.fdb_latexmk \
		makefileDependencies/*
	rm -rf auto

mrproper: clean
	rm -f *.pdf
