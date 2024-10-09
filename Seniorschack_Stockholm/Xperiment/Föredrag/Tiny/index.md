* Installation
	* python
	* makeAll.py
	* VS Code
	* Tanken är att all html genereras automatiskt då man sparar en fil.
		* Dessutom uppdateras fönstret i din webläsare.
* Publicera
	* T ex till Github eller annan server
* Katalogstrukturen motsvarar websidans struktur
	* båda är träd
	* Ge kataloger och filer vettiga namn, namnen kommer att synas!
* Börja med katalogerna
	* Kolla resultatet efter varje steg
		* Kör makeAll.py automatiskt eller för hand.
* Lägg till en fil, t ex .pdf-filer
* Lägg till en bild, t ex en .jpg-bild
* Lägg till en markdown-fil, index.md
	* Skriv in några ord
	* bold
	* italics
	* headlines
	* onumrerad lista
	* numrerad lista
	* indentera listorna
	* tabell
* style.css kan användas i varje katalog
	* Gäller i de underliggande nivåerna
	* testa t ex att ändra på någon färg

* Baserad på [markdown](https://www.markdownguide.org/cheat-sheet/).
* Anpassad för mobiler och äldre.
* Markdown kan ses för en sida genom att klicka på rubriken.
  * Ofta saknas .md, då är sidan skapad automatiskt mha kataloger och filer.
* Alfabetisk sortering av menyalternativen.
* Kronologisk sortering av Nyheter.
* Bakåt-knappen används alltid för att lämna en sida. (Alt + Left Arrow)
* Nya flikar skapas aldrig.
* Open Source på [Github](https://github.com/ChristerNilsson/2023/blob/main/023B-SeniorSchack/makeAll.py)

## .md 

This is a **markdown** file and is translated by *makeAll.py* to an **.html** file with the same name.

## .link

Files with this extension may contain a directory name, an html filename, a filename or an url.  
A **.link** file can be replaced by an **.md file**,  
but the user would see an extra menu level  
and thus have to use one extra *click*.  
You could say, the .link file acts as a shortcut.  

## From/To Matrix

| From/To | Dir | .md | .link | url |
|---------|-----|-----|-------|-----|
| Dir     | Yes | Yes | Yes   | Yes |
| .md     | Yes | Yes |       | Yes |
| .link   | Yes | Yes |       | Yes |
| url     |     |     |       |     |

**Yes**: a clickable link will be produced in the resulting html file.

* .md: ```[text](url)``` => ```<a href=url> text </a>```
* .link: Text file contains a url or file path
* url: Can also be any file except .md and .link
---
* .md can not refer to a .link.
* .link can not refer to another .link.
* In the produced .html file, .md and .link never occurs as targets.

## General advice

* Start with the folders
* Add files to your folders
* Add .link files to use urls
* Add an index.md file to show text, images and tables.
* Add an index.md file if you prefer another sort order
* Add html code to your .md files if necessary.
* Give all folders and files nice, short names, acceptable as menu names.
    * For the ```Nyheter``` folder, start all file names with a date, using the format YYYY-MM-DD.
* style.css can be used to customize your pages.
    * font
    * font size
    * colours
    * link decoration
    * paddings and margins
    * style.css can be defined in every folder.
        * Sheets closer to the leaf overrides sheets closer to the root.
        * Try changing color of the links in this folder: ```a {color:green}```
   	