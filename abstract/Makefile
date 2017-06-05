TEX = pandoc
src = template.tex abstract.yml
out = abstract.pdf
FLAGS = --smart --latex-engine=xelatex

all: $(out)

$(out) : $(src)
	$(TEX) $(filter-out $<,$^ ) -o $@ --template=$< $(FLAGS)

.PHONY: clean
clean :
	rm $(out)
