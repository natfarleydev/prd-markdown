BUILDDIR = ./build
FILES_MAIN = advancedIntro.markdown advancedRaces.markdown advancedBaseClasses.markdown advancedBaseClassesDetails.markdown advancedCoreClasses.markdown advancedCoreClassesDetails.markdown advancedPrestigeClasses.markdown advancedPrestigeClassesDetails.markdown advancedFeats.markdown advancedGear.markdown advancedSpellLists.markdown advancedSpellIndex.markdown advancedSpellDetails.markdown advancedMagicItems.markdown advancedMagicItemsDetails.markdown advancedNewRules.markdown # To make sure they're in order
FILES_ALL = $(FILES_MAIN) 

all: html epub

html: *.markdown # style.css Makefile
	pandoc -s --toc -o $(BUILDDIR)/pathfinder_advanced_players_guide.html $(FILES_ALL)
#	cp style.css $(BUILDDIR)

epub: *.markdown # style.css Makefile
	pandoc -t epub -o $(BUILDDIR)/pathfinder_advanced_players_guide.epub $(FILES_ALL)
# pandoc -t epub --epub-metadata=metadata.xml -s --epub-stylesheet=style.css --toc -o $(BUILDDIR)/book.epub $(FILES_ALL)

clean:
	rm -f $(BUILDDIR)/*.html
	rm -f $(BUILDDIR)/*.epub
	rm -f *.bak
