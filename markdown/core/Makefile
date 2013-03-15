BUILDDIR = ./build
FILES_MAIN = $(wildcard *.markdown)
# FILES_UPRAJNENIA = $(wildcard ./uprajnenia/*.markdown)
# FILES_RECEPTI = $(wildcard ./recepti/*.markdown)
FILES_ALL = $(FILES_MAIN) 
# .PHONY: clean spell

all: html epub

html: *.markdown # style.css Makefile
	pandoc -s --toc -o $(BUILDDIR)/test.html $(FILES_ALL)
#	cp style.css $(BUILDDIR)

epub: *.markdown # style.css Makefile
	pandoc -t epub --toc -o $(BUILDDIR)/test.epub $(FILES_ALL)
# pandoc -t epub --epub-metadata=metadata.xml -s --epub-stylesheet=style.css --toc -o $(BUILDDIR)/book.epub $(FILES_ALL)

info: *markdown
	pandoc -o $(BUILDDIR)/test.texi $(FILES_ALL)
	-makeinfo $(BUILDDIR)/test.texi -o test.info --force --error-limit=10000

clean:
	rm -f $(BUILDDIR)/*.html
#	rm -f $(BUILDDIR)/*.css
	rm -f $(BUILDDIR)/*.epub
	rm -f *.bak
