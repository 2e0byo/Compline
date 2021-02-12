cf=compline.tex
cfp=compline.pdf

ComplineLentFriday-book.pdf: $(cfp)
	pdfbook $(cfp)

$(cfp): $(cf)
	lualatex --shell-escape --interaction=batchmode $(cf)
	lualatex --shell-escape --interaction=batchmode $(cf) #compile twice for layout reasons
