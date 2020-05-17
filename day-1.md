# Web Fundamentals and Digital Humanities

> Tuesday, May 19th, 10:00am - 12:00pm, CDIL Zoom.

## Objectives

- Critical web literacy: `view-source`, markup languages, and Markdown.
- Critical understanding of collections as data.
- Literacy with digital files, data, and metadata.

# Outline:

## Introductions 

[What is Digital Humanities?](https://whatisdigitalhumanities.com/)

## The Web

- URLs (get code from servers): `https://example.com/about?key=value#anchor`
- Code: the web is made up of HTML, CSS, and JS (*mostly*), that is rendered in your browser.
    - "View page source" (right click any page), `view-source:`
    - "Inspect" (right click option) / Developer Tools (Ctrl + Shift + I)
    - "Plain text" ([file types note](https://evanwill.github.io/_drafts/notes/file-types.html))

## HTML Basics

> Demo using [JSFiddle](https://jsfiddle.net/)

**HTML (document / content / structure):**

*Hypertext Markup Language* is a ["markup language"](https://en.wikipedia.org/wiki/Markup_language) originally designed to describe documents for the web.
HTML is made up of a set of standard **elements** used to structure a web page and introduce features such as images.
Elements are represented by **tags** using point brackets, `<tag></tag>` that can be nested hierarchically.

- Doctype declaration: `<!DOCTYPE html>` (officially tells browser that it is an HTML file)
- Root element: `<html></html>` (all elements of a web page are nested inside the root element)
- Headers: `<h1></h1>`
- Paragraphs: `<p>text</p>`
    - Lorem ipsum text placeholder: [Lorem Ipsum classic](https://www.lipsum.com/), [Hipster](https://hipsum.co/), [Bacon](https://baconipsum.com/), [Cupcakes](http://www.cupcakeipsum.com/), [Pirate](https://pirateipsum.me/), [Corporate](https://www.cipsum.com/).
- Links: `<a href="link">link text</a>` (notice the *href*, this is an attribute that adds information to the element, in this case a link)
- Images: `<img src="imagefile">` (the *src* attribute is the path/link to an image file)
    - Find an image on the web (right click "view image")
    - Random image placeholder: [Picsum](https://picsum.photos/) add width and height like `https://picsum.photos/200/300`

**CSS (presentation / style):**

*Cascading Style Sheets* can be added to an HTML document in a `<style>` element, or loaded as a separate `.css` file.

- Element style: `h1 { color: red; }`
- Class: `<p class="big">Test</p>` / `.big { font-size: 25px; }`

**JS (interactivity / functionality):**

*JavaScript* can be added to an HTML document in a `<script>` element, or loaded as a separate `.js` file

- Add stuff: `<div id="example"></div>` / `var test = document.getElementById("example"); example.innerHTML = "Some example text.";`
- Click: `<button id="btn">Click Me</button>` / `var btn = document.getElementById("btn"); btn.addEventListener("click", function() { example.innerHTML = "You clicked the button!"; });`

## Markdown

> Demo to introduce Markdown and GitHub

- Log into [GitHub](https://gist.github.com/)
- Create a repository (click `+` button in upper right)
- Create a file in the repository
- Give it a filename with extension `.md`
- Write some markdown
- Commit (you are using Git)

- [Markdown basics](https://evanwill.github.io/write-md/content/2-markdown.html)
- [Markdown in a minute](https://evanwill.github.io/_drafts/notes/markdown-minute.html)
- [What is GitHub](https://evanwill.github.io/mini-web-crash-course/content/1-intro.html)

## Collections as Data

- [documents as data](http://history-lab.org/images/new-paper-stack.png) (from [History Lab](http://history-lab.org/)), using the lens of "data" to rethink traditional humanities research
- "Collections as data" are "readily open to computation", [The Santa Barbara Statement on Collections as Data](https://collectionsasdata.github.io/statement/)
- Philosophy for: research questions; collection planning; platform design
- [CollectionBuilder-GH](https://github.com/CollectionBuilder/collectionbuilder-gh)

# Follow up Activity

1. Explore interesting DH projects
    - [Reviews in Digital Humanities](https://reviewsindh.pubpub.org/)
    - See [list below](#DH-Projects)
2. Deconstruct content and platform. Think about source data, tools, outputs, and people.
    - e.g. Miriam Posner, [How did they make that?](http://miriamposner.com/blog/how-did-they-make-that/) 
    - Sustainability? (how many dead projects have you seen?)
3. Share your favorite example 
    - GitHub Issue in mini-symposium repository

# Additional Resources 

Workshops/tutorials: 

- [w3schools](https://www.w3schools.com/) (reference, tutorials, "try it" examples)
- [MDN web docs](https://developer.mozilla.org/en-US/) (good reference source)
- [Programming Historian](https://programminghistorian.org/)

## DH Projects

- [Kindred Britain](http://kindred.stanford.edu/)
- [American Panorama](http://dsl.richmond.edu/panorama/)
- [Republic of Letters](http://republicofletters.stanford.edu/)
- [Transcribing Bentham](https://blogs.ucl.ac.uk/transcribe-bentham/)
- [MarineLives](http://www.marinelives.org/wiki/Tools:_Collaboration_with_Transkribus)
- [Gendered Language in Teacher Reviews](http://benschmidt.org/profGender/)
- [Walt Whitman Archive](https://whitmanarchive.org/)
- [Profils 14 18](http://profils-14-18.tv5monde.com/#Introduction)
- [Slavery's Ephemera: The Contemporary Life of the Antebellum Plantation](http://vectors.usc.edu/projects/index.php?project=56)
- [Digital Archaeological Archive of Comparative Slavery (DAACS)](https://www.daacs.org/)
- [OpenContext](https://opencontext.org)
- [Digital Index of North American Archaeology](http://ux.opencontext.org/archaeology-site-data/)
- [Native Land](https://native-land.ca/)
- [Joods Monument](https://www.joodsmonument.nl/)
- [Plateau Peoples' Web Portal](https://plateauportal.libraries.wsu.edu/)
- [Mapping Indigenous LA](https://mila.ss.ucla.edu/)
- [Documenting Ferguson](http://digital.wustl.edu/ferguson/)
- [Documenting the Now](https://www.docnow.io/)
- [Digital Transgender Archive](https://www.digitaltransgenderarchive.net/)
- [Slave Societies Digital Archive](https://www.slavesocieties.org/)
- [The Real Faces of White Australia](http://invisibleaustralians.org/faces/)
- [Mapping Massacres](https://c21ch.newcastle.edu.au/colonialmassacres/map.php)
- [Torn Apart/Separados](http://xpmethod.plaintext.in/torn-apart/volume/1/)
- [Viral Texts](https://viraltexts.org/), mapping periodical reprinting 19th cent.
- [Chinatown Sound Map](http://chinatownsoundmap.com/about/)
- [Frankenbook](https://www.frankenbook.org/)
- [DIY History](https://diyhistory.lib.uiowa.edu/), crowd/student transcription.
- [Topic Modeling Martha Ballard's Diary](http://www.cameronblevins.org/posts/topic-modeling-martha-ballards-diary/)
- [Mining the Dispatch](http://dsl.richmond.edu/dispatch/), topic modeling fugitive slave ads from the Richmond Dispatch
- [Coins](https://uclab.fh-potsdam.de/coins/)
- [The World's Writing Systems](http://www.worldswritingsystems.org/)
- [Historic Tale Construction Kit](https://htck.github.io/bayeux/)

-----------------------

> Outlines: [0](day-0.md) | [1](day-1.md) | [2](day-2.md) | [3](day-3.md)
