# HACKtivity

### Before we start

- If you're **getting stuck** or falling behind, please tell me straight away. Sometimes it's just a matter of a missing semi-colon or so..
	
- If you have an **idea** and want to know how to code it, I may not answer that immediately but note it down and we'll crack it later.



### Let's code

1. Search for Webmaker
* Go to Webmaker and sign in (with Persona)
* Search for [Web comic template](https://webmaker.org/en-US/search/?type=all&q=web+comic+template), hit **Remix** 
* Create `<html>`, `<head>` and `<body>` as the **skeleton** of every and any webpage. **Like a person**, it has a head and a body.

 	`<body>` is the visible part of an HTML page. 
* Make a `<p>`, make it about your chosen topic (*what if*, *what is* or *how to*).
* Save and preview
	
	**Pay attention here** If you add `_` at the end of the published URL you get a clean, iframe-less comic.

- **Show the finished comic**. 

	We've got our first line, next step is to create the basic structure of the comic. 
	
	Each key moment in a comic is framed by a **panel**, each **section** of the comic is a panel.
	
	In HTML we have an element called `section` which we can use to frame things.

- Create an **empty panel/section**. 

        <section>
	    </section>	
	    
* **Comment** that. 

* Let's **add images** to get our comic off the ground.

	We'll use the browser-waiter image from IMGUR.
	![](http://i.imgur.com/Seem5xZ.png)
	
	Point people to **[baddeo.imgur.com](http://baddeo.imgur.com)** (later in the day they'll be able to use their own images)
	
	**Nest it** inside the first panel.
	
* Ask **students to make another panel** under the first one.	
* Ask **students to add another image**.
	
	We'll use the server-chef image from IMGUR.
	![](http://i.imgur.com/CxzZKlF.png)	
	
* Now that we have images, we can start writing our story. 

	In comics, you can use **speech bubbles** to make your characters "talk".	
	
* Add **one paragraph** to the first section, and **two paragraphs** to the second section.

	`<p class="bubble">Hello, I'm your browser. What do you want?</p>`
	
	`<p class="bubble">I'm the server, just got an HTTP request from the browser</p>`
	
	`<p class="bubble">Now I'm cooking an HTML page</p>`
	
* Create the **third panel/section**.

* Add the happy browser to it
	
	![](http://i.imgur.com/s4apyQC.png)
	
* Add a **speech bubble** to the third panel/section.	
	`<p class="bubble">Here's your page as requested. Would you like a cookie with it?</p>`
	
* Add a **link** to a page that explains what cookies are. **Ask students to search** and find out. Then **paste** their URL of choice inside their comic.	

	`<p class="bubble">Here's your page as requested. Would you like <a href="http://www.bbc.co.uk/webwise/guides/about-cookies">a cookie</a> with it?</p>`
	
* Create the **fourth panel/section**.

* We want to **embed** another web-page into our comic. 

	We can use `iframe` to do that.
	
	`<iframe src="https://blabla.com"></iframe>`
	
	This allows you to embed pretty much anything into a web-page.
	
	There's a **limitation** on Thimble (it only seems to work with websites served over `https`, unless you change the address to `http`)
	
	Also **some companies don't allow** you to embed their websites. For instance if you want to embed something from Twitter, you can't simply paste the URL into it but have to follow their instructions.
	
	
	
	
	
	

### Take a **break**!	
	
	
	
	
	
	
	
	
	
1. Now we've got **all our content marked-up**. 

	So we're **done with HTML**, the browser knows about all the content of our comic.
	
	But the browser doesn't know how to **style** it. It simply **stacked** all the ingredients of our comic one on top of one another. We need to change that, right? 

* Let's **save** and head over to the *Inspect tab*.

- Right-click, `Inspect Element`. 

	This is the **Web Inspector**, where you can see every page's *source code*, *styles* and much more. 
	
	When you hover over the source code with your mouse, the corresponding HTML element on the page will light up. 
	
	When you click on an HTML tag in the source code (on the **left**), you'll see all its styles (on the **right**).


	On the **left** of the Inspector we can see the HTML code of our comic.
	
	On the **right** there's the style. Well there's not much of it atm.
	
* Add a `background: yellow;` to the first panel, then to the second and third panel.. this is a **pain**! 

	We need a way to tell the browser to style all the panels the same way. Some sort of **style guide** or **dress code**..
	
	Meet **CSS**. It stands for ***C**ascading **S**tyle **S**heets* and it's the **language** you can use to tell your browser to change colours, sizes and many other **stylistic** aspects of your HTML documents.
	
	
* Copy the `element.style {...}` from the Inspector into the *Editor tab*, inside the `<style>` in the `<head>`.	
	
	We want to tell the browser to give **every section** a yellow background.
	
	Change `element.style` to `section`
	
	    section
		{
			background: yellow;
		}
	
	Point out that this is a different language, with a **different grammar**. 
	
	HTML is for **content and structure**.
	
	CSS is for **style and design**.
	
	
* Let's give our comic a balanced, **centred layout**. 

		body
		{
			max-width: 600px;
			margin: auto;
		}	
	
* **Ask students** how we can go about **styling the speech bubbles**. 

	Since we gave all our speech bubbles a `class` name, we can now target them specifically like this with CSS
	
	`p.bubble {}` 
	
	Point out that it's **good practice** to always open and close the **curly brackets** to avoid forgetting it and confusing the browser.
	
	  p.bubble
      {
        background: pink;
        padding: 10px;
        margin: 0px;
      }
  
* Add `margin` to **separate** the panels.
		
		margin-bottom: 10px;  

* How do you **make different voices**? You're all dying to change the default look of your texts.
	
	Search for *Google Fonts*
	
	Pick one font quickly, you can change it later..
	
	Follow the instructions to include your chosen font in your page.
	
	Remember to change the `http` in the GF link to `https`
	
	
### Take another **break**!	

* Now we want to **position** our speech bubbles inside the panels.

	First of all, let's give our speech bubbles `id` names, as their position will be differents.

	We want to say something like "browser, **offset** this speech bubble 50px from the top".
	
	`top: 50px;`
	
	And the browser will say "ok, but 50px from the **top of what?**"
	
	So we want the browser to disregard the order in which the speech bubbles appear in the HTML, to be **absolute**
	
	`position: absolute;`
	
	The bubbles fly off, so we need to set them *relative* to their parent sections. 
	
	`position:relative;`
	

	`position` defines how an element can be moved with **offsets** (`top`, `right`, `bottom` and `left`).
	
	`position:relative` offsets an element in relation to **itself**
	
	`position:absolute` offsets an element in relation to its **first, non-static ancestor**    




## Optionals


* **Ask students to embed a Google map** in their comic.
* **Ask students to embed a Twitter widget** in their comic.

* **Floats**

* **Overflows**

* **Border-radius**


* Give your comic a heading `<h1>` and a subheading `<h2>` 

	Maybe introduce `<b>` and `<i>`?
	
* Make the arrow


        .bubble:after
    	{
    		content: " ";
			position: absolute;
		
			border-width: 30px;
			border-style: solid;
    	}
    
    	#panel1 .bubble:after 
		{
			top: 100%;
			left: 30px;
			
			border-top-color: white;
			border-left-color: red;
			border-bottom-color: green; 
			border-right-color: blue; 
		} 		

	
	 
	
	




	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
## OLD	
	
	

* Save and go to the *Inspect tab*. Point out that the `<section>` is there but it has **zero height**.

* Make the *empty* panel visible on the right side of the Inspector.

	`element.style { height: 300px; background: yellow; }`


* Copy the style from the Inspector into the *Editor tab* to get styling.

	Point out that this is a different language, with a **different grammar**. 

 
	**CSS** stands for ***C**ascading **S**tyle **S**heets* and it's the language you can use to tell your browser to change colours, sizes and many other *stylistic* aspects of your HTML documents.
	
        section 
        {
        	background-color: yellow; 
        	
        	remember to spell out the colon and semi-colon
        	
        	height: 300px;
        	
        	width: 100%; 
        	required? yes because we'll add a float:left; later
        }
               



 * Add `margin` to **separate** the panels.
		
		margin-bottom: 10px;
		
* Now, empty panels don't really tell a story, do they? Let's **add images** to get our comic off the ground.

	Find an image on Google, or **upload one to [IMGUR](http://baddeo.imgur.com)** (get people to sign in to IMGUR first), then *nest it* inside a panel.

	We'll use the browser-waiter image from IMGUR.
	![](http://i.imgur.com/Seem5xZ.png)

* Uh-oh, we have an image that is too big for its panel.

        overflow: hidden;
        
        and mention 
        width: 100%;
        
* By default the image sticks to the top-left corner of its parent. 

 	We can **offset** it with `top` and `left`.
 	

 	
* We want it to **stick** to the right of its panel. Let's use `position:absolute` with `right` and `bottom`
 	
 	This a good point to introduce `id` attributes
 	
 	Using the `id` attribute you can *identify* your HTML elements. **`id` names are entirely up to you**.  An id is *unique*, just like you :)

* Now that we have images, you can start writing your story. In comics, you can use **speech bubbles** to make your characters "talk".

	Introduce class names for speech bubbles (a special *type* of `<p>`s)

        p.bubble
        {
    	    background-color: white;
    		padding: 10px;
    		
    		position: absolute;
    		
    		margin: 0; (to remove the default browser style)
    	}
    	
  Using the `class` attribute you can *classify* your HTML elements. **`class` names are entirely up to you**. 
    	
* **Offset** the speech bubble. 
* **Students make another speech bubble** for the other panel
* Realise that the rules we've added to `p.bubble` apply to this new bubble, correct the situation with `id` 
* Maybe add `id` to the `<section>` elements and introduce slightly more complex CSS selectors 

* How do you get **many panels on the same row**?

	First **make 2 panels** and set their `width` values to eg: `300px` and `300px`
	
	Then add `float: left;` inside the `section` rule
	
	Give the left panel a `margin-right: 10px;` and adjust its `width`;
	
* Add the happy browser to the third panel
	
	![](http://i.imgur.com/s4apyQC.png)
	
* Add the web-page to the fourth panel
	
	![](http://i.imgur.com/mE0P5AB.jpg)	

* How do you get an image to take all the available space in the panel, without loosing its aspect ratio?

        background-image: url("http://i.imgur.com/mE0P5AB.jpg");
        background-size: cover; (and/or contain)
        
* How do you **make different voices**? You're all dying to change the default look of your texts.
	
	Search for *Google Fonts*
	
	Pick one font quickly, you can change it later..
	
	Follow the instructions to include your chosen font in your page.
	

 





	


	


## 

# Notes

### About the code
* ~~Do we need the `padding-left: 10px` on the body? No.~~
* Do we need `width: 100%` on section? Yes, for the float later.
* Maybe we don't need to classify the panel? it can be just a `<section>`. OK
* Why can't we use `margin` instead of `border-bottom`? Let's use margin.
* ~~Do we need the `border-right` for the panel? No~~
* ~~Find an image that is bigger that 300px high~~
* ~~Should we give a border to our panels, rather than a yellow background? Nah~~
* How to explain **absolute** positioning?

	`position` defines how an element can be moved with **offsets** (`top`, `right`, `bottom` and `left`).
	
	`position:relative` offsets an element in relation to **itself**
	
	`position:absolute` offsets an element in relation to its **first, non-static ancestor** (since we've defaulted * to `position:relative` we can simply say that `absolute` offsets an element in relation to its **parent**)

* How to explain the **float** property? 
	
	By default, you can have one HTML *block* element per "line".
	
	With `float:left` we can tell them to **snap** to the left of the available space in the "previous line".
	
* How to explain **cover/contain** background-size?

	**contain**

    The background image is scaled, while preserving its proportions, so as to be as large as possible providing that it is *contained* within the background positioning area. 

    **cover**

    The background image is scaled, preserving its proportions, to be as large as possible so that the background positioning area is *completely covered* by the background image

* ~~Do we need *How do you **make a speech bubble arrow**?* eg: Noble Denim~~

##### 10.09

* No need to change the `<title>` at the beginning, it seems to confuse people (as it's not immediately visible). They'll change it later by themsleves, also they don't really know what they may want to title their comic so it's a big ask at the beginning.

* When introducing `position:absolute` some people's images will fly off, because they're not inside `<section>`














### About the tutorial

* Encourage students to **note down their questions** and answer them later (unless they're stuck and something is not working).

* Point out that comments are useful to take notes, and to hide code from the browser.. and comment code as you go along

* Encourage students to search for HTML and CSS solutions on the Web (Stack Overflow)

* If students get stuck, they can work together on the same project by hitting their username on the top-right, then clicking on *Collaborate* (it will slow down the browser but it can be useful for debugging)

* Mention [Dash](https://dash.generalassemb.ly/) and [Codecademy](http://www.codecademy.com/) for those who want to take their coding further.


#### 10.09

* Maybe we start from a *blank* template? Add a `<section>` then save, view it in a new tab. 
	
	**Inspect it**. This way we can introduce styling. Copy the `element.style {
background: yellow;
height: 300px;
}` from the Inspector into their project to get stylin'

* Get them to follow me and use the same images etc, and then set them free in the afternoon?

* Maybe a whiteboard to **sketch out / wireframe** the comic would be helpful? Or I could show them what we're aiming to do together (something like [the finished comic](https://baddeo.makes.org/thimble/ODI3NTg4ODY0/the-www-restaurant)), explaining what we're going to learn by making it.

* Give `id`s to sections from the start, so that we do it the right way. Maybe introduce `id` on the section by giving it a different `background`.

* Make 2 speech bubbles in the same panel, then `position` them

* `id` and `class` names should be simple, `panel1` is bettern than `panel-1` for instance

* One student said a print-out cheat-sheet of sorts could be helpful

* Embed a youtube video, a Google map and a Twitter feed after the `float:left` task. We can start by embedding a whole page via iframe (instead of another image)

* We need to get people as close to the projector as possible. Also a close, quiet room works better than an open space. 

* Point out that we can remix other people's comics so if you're falling behind you can catch up that way.

- [x] I don't want to discourage people from asking questions, but some of them I can postpone to answer later. Maybe make the rules clear at the beginning of the coding session.

	*If you're **getting stuck** or falling behind, please tell me straight away. Sometimes it's just a matter of a missing semi-colon or so..* 
	
	*If you have an **idea** and want to know how to code it, I may not answer that immediately but note it down and we'll crack it later.* 
	
* Need to **show comments** in HTML and CSS and explain why they're useful. Make a point to use a comment at the beginning and then try to use them throughout.	

#### 11.09 

* Set the browser tabs to 125% (Editor) - 200% (Inspect) zoom











### About Thimble

* When the preview reloads it shouldn't scroll to the top of the page but *remember* where we've scrolled
* Embedding Google Fonts may generate a "400" Failed to load resource (Bad request): can be solved by removing `http:` in the the Google Font CSS link href `<link href='//fonts.googleapis.com/css?family=Open+Sans' rel='stylesheet' type='text/css'>`
* It would be great to have separate files for CSS and HTML 
* It would be very useful to be able to collapse elements, both for explanation purposes and to declutter your page while you work..
* If you misspell `absolute` it doesn't turn red
* If you have 2 }} it doesn't turn red
* Keep getting an error when trying to save [this Maker Party Report](https://baddeo.makes.org/thimble/maker-party-report).

