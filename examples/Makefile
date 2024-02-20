source      := chronicles-example.adoc
target_pdf  := chronicles-example.pdf
target_html := chronicles-example.html

asciidoctor_pdf := $(HOME)/.ruby_gems_perso/bin/asciidoctor-pdf

all: $(target_pdf) $(target_html)

$(target_pdf): $(source)
	$(asciidoctor_pdf) -r asciidoctor-mathematical -r asciidoctor-diagram $(source)

$(target_html): $(source)
	asciidoctor -r asciidoctor-mathematical -r asciidoctor-diagram $(source)

clean:
	rm -f $(target_pdf) $(target_html)

.PHONY: all clean

