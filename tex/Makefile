NAME=xpmahut00

all: $(NAME).pdf

$(NAME).pdf: clean
	pdflatex $(NAME)
	bibtex $(NAME)
	pdflatex $(NAME)
	pdflatex $(NAME)

clean:
	rm -f *.dvi *.log $(NAME).blg $(NAME).bbl $(NAME).toc *.aux $(NAME).out $(NAME).lof
	rm -f $(NAME).pdf
	rm -f *~

show: $(NAME).pdf
	evince $(NAME).pdf
