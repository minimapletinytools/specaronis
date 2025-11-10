# AI Manga Reader for Learning Japanese

# High Level Overview

- loads digital manga/graphic novels 
- uses OCR to detect chunks (e.g. a speech bubble) of Japanese language text and the exact location each charcter in the chunk
- uses AI to translate the original text
- uses AI to break down the chunks into logical groupings of words
- uses AI to explain each grouping
- uses AI to explain the entire chunk of text
- provides a simple UI to view the original images, AI translations and explanations

## App Navigation Functionality
- (P0) Main website has an "upload" button allowing user to upload their manga
- (P0) after uploading, generates a unique shareable URL schema allowing user to read the uploaded manga at a specific page
- (P0) Supports uploading manga
    - (P0) zipped folders of png/jpg images 
    - (P2) Supports CBZ/CBR/PDF
- (P1) Supports caching and storage of all AI translation and explanations 
- (P2) Supports user login and the following user based functionality
    - (P2) manage uploads (share, delete, etc)
    - (P2) recent uploads, recent views, tracks last page read, etc
    - (P3) sharing settings on user upload ()

    
## Viewer Functionality 
- (P0) on hover functionality
    - hover over groupings in a chunk displays translation for that grouping
    - hovering on the border of the chunk displays translation for the entire chunk in a box to the right of the chunk (so they can be seen side by side)
- (P1) info panel shows to the right of the entire image that contains translation information
    - (P1) clicking on grouping displays translation for the grouping and has AI explain it
    - (P1) clicking on border of a chunk displays translation for the entire chunk and has AI explain it
    - (P2) clicking on border of the entire image has AI attempt to explain the entire image in context of the entire manga
- (P1) Supports translation settings, grouping detail level 1-5 (e.g. 1: individual words, 5: complete sentences)
- (P1) Supports AI explanation settings (i.e. different prompt settings to control the level of detail in the AI explanations)
- (P2) Overlay optional toggle
    - toggle to overlay english words on top of original japanese text (sort of like where pinyin would go)
    - toggle to completely overlay english translation in the orginal chunks location
