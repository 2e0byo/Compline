PHONY: all

all: compline.pdf compline-booklet.pdf

compline.pdf: compline.tex
	env openout_any=a latexmk --shell-escape --pdflatex=lualatex --pdf compline.tex

compline-booklet.pdf: compline.pdf
	pdfjam --landscape --suffix booklet --booklet true  compline.pdf

