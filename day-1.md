# Web Fundamentals and Digital Humanities

> Tuesday, May 19th, 10:00am - 12:00pm, CDIL Zoom.

## Objectives

- Critical web literacy: `view-source`, markup languages, HTML basics.
- Introduce GitHub and Markdown.
- Introduce collections as data.

# Outline:

## Introductions 

[What is Digital Humanities?](https://whatisdigitalhumanities.com/)

## The Web

- **Network:** a network is infrastructure for computers to communicate, *The Web* is a network of networks!
- **URLs:** web addresses that request code from servers, `https://subdomain.example.com/about/index.html?key=value#anchor`
- **Code:** the web is made up of HTML, CSS, and JS (*mostly*), that is rendered in your browser.
    - "View page source" (right click any page), `view-source:`
    - "Inspect" (right click option) / Developer Tools (Ctrl + Shift + I)
    - "Plain text" ([file types note](https://evanwill.github.io/_drafts/notes/file-types.html))

## HTML Basics

> Demo using [JSFiddle](https://jsfiddle.net/) to introduce the fundamental material of the web.

**HTML (document / content / structure):**

*Hypertext Markup Language* is a ["markup language"](https://en.wikipedia.org/wiki/Markup_language) originally designed to describe documents for the web.
HTML is made up of a set of standard **elements** used to structure a web page and introduce features such as images.
Elements are represented by **tags** using point brackets, `<tag>content</tag>` that can be nested hierarchically.

- Doctype declaration: `<!DOCTYPE html>` (officially tells browser that it is an HTML file)
- Root element: `<html></html>` (all elements of a web page are nested inside the root element)
- Head: `<head></head>` (provides metadata for the document)
- Title: `<title></title>` (nested inside the head, you will see it at the top of your browser tab)
- Body: `<body></body>` (the content to be displayed)
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

- Add stuff: `<div id="example"></div>` / `var example = document.getElementById("example"); example.innerHTML = "Some example text.";`
- Click: `<button id="btn">Click Me</button>` / `var btn = document.getElementById("btn"); btn.addEventListener("click", function() { example.innerHTML = "You clicked the button!"; });`

Example HTML doc:

```
<!DOCTYPE html>
<html>
    <head>
        <title>Example HTML</title>
        <style>
            h1 { color: red; }
            .big { font-size: 25px; }
        </style>
    </head>
    <body>
        <h1>Header One</h1>
        <p>Some text in a paragraph.</p>
        <p>A link to <a href="https://github.com/thecdil/mini-symposium">Symposium</a>.</p>
        <p class="big">Test</p>
        <div id="example"></div>
        <p><button id="btn">Click Me</button></p>
        <img src="https://www.lib.uidaho.edu/media/digital/small/ott.jpg">
        <script>
            var example = document.getElementById("example"); 
            example.innerHTML = "Some example text.";
            var btn = document.getElementById("btn");
            btn.addEventListener("click", function() { example.innerHTML = "You clicked the button!"; });
        </script>
    </body>
</html>
```

## GitHub 

[GitHub](https://github.com/) is a cloud [Git](https://git-scm.com/) repository hosting service with builtin features for collaboration and project management.
Think of it as Google Drive for code with super robust "track changes" baked in.

It is the most popular platform for developing and sharing code from enterprise projects, to hands-on learning, to academic projects.
Thus, it is helpful to get familiar with the web interface so that you can take part in this community.

One amazingly useful GitHub feature is [GitHub Pages](https://guides.github.com/features/pages/), a free static web hosting service, great for learning, messing around, and publishing your work.

## Markdown 

> Demo to introduce Markdown and GitHub.

[Markdown](https://daringfireball.net/projects/markdown/) is a standard to simplify writing content for the web.
A handful of simple conventions translate into the basic HTML elements, making it quick to write and edit. 
Markdown can be used any where on GitHub, in popular static site generators such as Jekyll, and to create documents using [Pandoc](https://pandoc.org/) or a Markdown editor.

- Log into [GitHub](https://github.com/)
- Create a repository (click `+` button in upper right)
- Create a file in the repository (click "Create new file")
- Give it a filename with extension `.md`
- Write some Markdown in the editor (see [Markdown basics](https://evanwill.github.io/write-md/content/2-markdown.html))
- Scroll down to Commit (you are using Git!)

## Collections as Data

- [documents as data](http://history-lab.org/images/new-paper-stack.png) (from [History Lab](http://history-lab.org/)), using the lens of "data" to rethink traditional humanities research
- "Collections as data" are "readily open to computation", [The Santa Barbara Statement on Collections as Data](https://collectionsasdata.github.io/statement/)
- Philosophy for: research questions; collection planning; platform design
- [CollectionBuilder](https://collectionbuilder.github.io/)

# Follow up Activity

1. Explore interesting DH projects
    - [Reviews in Digital Humanities](https://reviewsindh.pubpub.org/)
    - See [list below](#DH-Projects)
2. Deconstruct content and platform. Think about source data, tools, outputs, and people.
    - e.g. Miriam Posner, [How did they make that?](http://miriamposner.com/blog/how-did-they-make-that/) 
    - Sustainability? (how many dead projects have you seen?)
3. Share your favorite example 
    - [GitHub Issue in mini-symposium repository](https://github.com/thecdil/mini-symposium/issues/1)

## Reading for Tommorrow 

- <http://kindred.stanford.edu/notes.html?section=originating>
- <http://kindred.stanford.edu/notes.html?section=designing>
- <http://kindred.stanford.edu/notes.html?section=developing>

## DH Projects

Texts:

- [Perseus Digital Library](http://www.perseus.tufts.edu/hopper/) - classical texts since before the internet!
- [Walt Whitman Archive](https://whitmanarchive.org/), [Melville Electronic Library](https://melville.electroniclibrary.org/), [Rossetti Archive](http://www.rossettiarchive.org/), [William Blake Archive](http://www.blakearchive.org/), [Newton Project](http://www.newtonproject.ox.ac.uk/) - traditionally canonical authors supported big projects, interesting opportunity to bring together published and archival materials with multimedia and scholarly content. [Willa Cather Archive](https://cather.unl.edu/) is a recent, very complete example.
- [Eighteenth-Century Poetry Archive](https://www.eighteenthcenturypoetry.org/) - many projects gather together a thematic corpus of text.
- [Women Writers Project](https://wwp.northeastern.edu/) - some projects seek increase visibility of hidden creators.
- [Digital Thoreau](https://digitalthoreau.org/), [Petrarchive](http://dcl.slis.indiana.edu/petrarchive/index.php) - new ways to open up critical editions.
- [Reading Like a Victorian](http://victorianserialnovels.org/) - represent original serial access to novels.
- [Frankenbook](https://www.frankenbook.org/) - collaborative reading text.
- [Visual Haggard](http://www.visualhaggard.org/) - extracting illustrations rather than text.

Digging into the archives:

- [Collective Biographies of Women](http://cbw.iath.virginia.edu/index.php) 
- [London Lives](https://www.londonlives.org/)
- [Mining the Dispatch](http://dsl.richmond.edu/dispatch/) - topic modeling fugitive slave ads from the Richmond Dispatch.
- [Joods Monument](https://www.joodsmonument.nl/)
- [Robots Reading Vogue](http://dh.library.yale.edu/projects/vogue/)
- [Historic Tale Construction Kit](https://htck.github.io/bayeux/)
- [17th century death roulette](https://vole.wtf/death-roulette/)

Networks:

- [Victorian Web](http://www.victorianweb.org/index.html) - pre-web hyperlinked text project.
- [Kindred Britain](http://kindred.stanford.edu/)
- [Republic of Letters](http://republicofletters.stanford.edu/)
- [Six Degrees of Francis Bacon](http://www.sixdegreesoffrancisbacon.com/)

Mapping:

- [American Panorama](http://dsl.richmond.edu/panorama/)
- [Native Land](https://native-land.ca/)
- [Mapping Indigenous LA](https://mila.ss.ucla.edu/)
- [Mapping Massacres](https://c21ch.newcastle.edu.au/colonialmassacres/map.php)
- [Viral Texts](https://viraltexts.org/), mapping periodical reprinting 19th cent.
- [Scottish Witches](https://witches.is.ed.ac.uk/)
- [Chinatown Sound Map](http://chinatownsoundmap.com/about/)
- [Navigating the Green Book](http://publicdomain.nypl.org/greenbook-map/)
- [The Garden of Earthly Delights interactive adventure](https://archief.ntr.nl/tuinderlusten/en.html)

Active history:

- [Torn Apart/Separados](http://xpmethod.plaintext.in/torn-apart/volume/1/)
- [Documenting Ferguson](http://digital.wustl.edu/ferguson/)
- [Documenting the Now](https://www.docnow.io/)

Digital collections:

- [Plateau Peoples' Web Portal](https://plateauportal.libraries.wsu.edu/)
- [Digital Transgender Archive](https://www.digitaltransgenderarchive.net/)
- [Slave Societies Digital Archive](https://www.slavesocieties.org/)
- [The Real Faces of White Australia](http://invisibleaustralians.org/faces/)
- [RE Activate Mama Pina's Cookbook](http://www.criticalmediartstudio.com/RemediatingMamaPina/)
- [DIY History](https://diyhistory.lib.uiowa.edu/), crowd/student transcription.
- [Digital Archaeological Archive of Comparative Slavery (DAACS)](https://www.daacs.org/)
- [Coins](https://uclab.fh-potsdam.de/coins/)

# Additional Resources 

- Miriam Posner, ["Humanities Data: A Necessary Contradiction" (2015)](http://miriamposner.com/blog/humanities-data-a-necessary-contradiction/)

Workshops/tutorials: 

- [w3schools](https://www.w3schools.com/) (reference, tutorials, "try it" examples)
- [MDN web docs](https://developer.mozilla.org/en-US/) (good reference source)
- [Programming Historian](https://programminghistorian.org/)

-----------------------

> Outlines: [0](day-0.md) | [1](day-1.md) | [2](day-2.md) | [3](day-3.md)
