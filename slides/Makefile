all:
	pandoc -f markdown slides.md -t revealjs --standalone --css=custom.css -o index.html -V mouseWheel=true -V history=true -V controls=false -V slideNumber=true -V slideNumber='"c/t"'
	ruby fix_images.rb
