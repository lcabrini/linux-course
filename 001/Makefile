ASCIIDOCTOR = asciidoctor-pdf
WORKBOOK = linux-001-workbook.pdf
PRESENTATION = linux-001-presentation.pdf
PDF = $(WORKBOOK) $(PRESENTATION)
THEME = -a pdf-style=../theme/presentation-theme.yml

all: $(PDF)

$(WORKBOOK):
	$(ASCIIDOCTOR) workbook.adoc -o $@

$(PRESENTATION):
	$(ASCIIDOCTOR) presentation.adoc $(THEME) -o $@

clean:
	$(RM) $(PDF)
