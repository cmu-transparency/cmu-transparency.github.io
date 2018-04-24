PEOPLE := alexandra alfred amit anne anupam arthur caleb daniel david gihyuk helen \
	jeannette klas matt michael ole piotr raj shayak saikat sam \
	sophia tom caleb 

PEOPLE_IMAGES := $(PEOPLE:%=%.jpeg)
PEOPLE_THUMBS := $(PEOPLE:%=thumbs/%.jpeg)

thumbs: $(PEOPLE_THUMBS)

thumbs/%.jpeg: %.jpeg thumbnail_faces.py
	python3 thumbnail_faces.py $*.jpeg thumbs/$*.jpeg \
		--width 400 --height 500
