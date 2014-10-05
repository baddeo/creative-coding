# Notes

### 12.09

#### Presentation

* [x] `src` is not `scr` (maybe we have that as part of the *Spot the difference* activity)
* *Spot the difference* could also have missing or double `}}`
* [x] Let them know at the beginning when they're going to have **breaks**, otherwise they get distressed and wet themselves.
* [x] Use the **sandwich analogy** to explain html tags
* [x] ~~Visuals for the building blocks of a comic may help in the presentation?~~
* [x] Need to find a smoother way to go from WEB (comic) to WWWTF? What is the Web in a nutshell, how it started and how does it work..

#### Hacktivity

* [x]Explain that we're going to work on **content and structure first**, **then style** it. Show the final result, then a version without style. 
* Make sure people are using the same browser I'm using (not IE please).
* Explain the **DRY** principle when introducing CSS.
* A good coder is a **lazy coder**: **copy-paste** whenever you can, use **shortcuts**.
* Tell them that **positioning is tricky**, but understanding it will allow them to control their comic layout with extreme precision. 
* Point out that **position** is going to be the **trickiest** part of the session, maybe ask them to just look at me coding for a minute, and then try and reproduce the 3 steps (also commenting those steps in the CSS may help). Still can't find a good way to explain it. Maybe we re-introduce ` * { position: relative; } ` in the template? 
* always use **px**, not just 0
* [x] In the slide about **copy-hack**, maybe we loose the facebook thing (you can show it when we're introducing the web inspector) and instead say something like "copy me (before lunch), then hack it (after lunch)"
* [x] When I'm saying that "learning to code is like learning a new language", mention that **today** you're going to learn **2 new languages**
* Ask more **why** questions, ask students to explain what they're doing, to see if they understand what each line of code does.
* Ask people to **google for solutions**
* You can customise your **Tumblr**, maybe instead of talking about *makers vs consumers* I could make more practical examples of what they can do with what they'll learn today.
* If we set `top:50px;` and then `bottom:0px;` the speech bubble stretches over the height of its parent..
* When setting images with `position:absolute;` their parent section will collapse. A quick work-around is to set the parent's `height`
* If we start late, we're going to leave late.. so really is up to you.
* Later in the afternoon you can let them *code* [Flappy Bird](http://studio.code.org/flappy/1)
* Before students can leave they have to send their comic's link to me.
* People seem to like the browser-server illustrations, they find them *cute*.
* Make a point that everything you want people to see has to be within the `<body> </body>`.
* Didn't get to use **classes** at all today. Maybe `p.bubble` should be used instead of `section p`
* Explaining `id` attributes as a way to talk specifically to one person as opposed to all the class seemed to work well. Especially when I pointed at a random person and asked "What's your name?" 
* Maybe `class` could be used with a peoples' analogy, eg `class="male"`
* Switching between *panel* and *section* doesn't help, maybe just use `section`
* Stress that `_` at the end of the URL of their comic is super-important, cause if you don't put it you'll get confused and you'll cry.


### 17.09

* If I promise people to have breaks at certain times, I should stick to those. Otherwise I can tell them that we'll have lunch when we get to a certain check-point.
* Maybe we should have a **to-do** list so that people know what we're aiming for (on Github or Wunderlist?).
* **Horseshoe** class layout works better than rows.

#### Presentation

* [x] Why do we need code? What is code used for? Who or what runs code?
* [x] Ask less questions, eg: *How do you learn to code?* doesn't yield good answers, it's rather vague
* Start presentation by saying *I'm going to ask you a few questions before we get hands-on with code*
* [x] Re-jig the *How to learn code* slide, stressing that you'll learn 2 languages, then talk about copying and hacking.
* [x] Guessing HTML is hard, especially the M part. Need to find a way to ease people into it
* [x] Explain what marking up means, eg *telling the browser "this is an image, this is a paragraph etc"*
* Stress that **code is a tool**, is how we can get computers to do the **heavy lifting for us**, so that we can focus on being creative.


* Get people to choose the subject of their comic early on, by giving them some constraint, eg pick from [Google Zeitgeist UK 2013](http://www.google.co.uk/trends/topcharts?date=2014#geo=GB&date=2013), you have five minutes to discuss and choose a topic (from the *What is..* and *How to..* categories), or make one up and convince everybody that it's worth a comic. Do a bit of planning before we jump into coding.
* Or maybe give them a **random letter** and they choose a theme starting with that letter? Or use a [random word generator](http://www.wordgenerator.net/noun-generator.php)?

#### Hacktivity

* [x] Facebook hacking is a *wow* moment!
* Let's try and do a *spot the difference* between the unstyled comic and the finished comic side by side. Good, worked well.
* Re-introduced the `class` attribute for `.bubble`, explain it with people's classes (male/female etc.), then use first names to explain `id`. Maybe a pseudo-code example could work?

        <person class="female student" id="ruby"></person>
		    
* Gave margin to bubble before adding the marging to the sections
* Make sure you've got only one `<body>`
* Make sure bubbles are inside sections
* Show `top`, `left`, `bottom` and `right`, not just two of them. 
* People don't seem to get the CSS selectors, maybe we could do a bit of a **translation quiz** 
* Ask people to refrain from styling the texts with `<font>`, tell them you'll show them how to tackle that after lunch.

### 18.09
 
* Point out that all the (Webmaker, IMGUR, Google Fonts) (Webmaker, IMGUR, Google Fonts) we're using are **free and easy to use** 
* [ ] Introduce the HTML5 (dog) glossary? What about StackOverflow?
* **Smile**!
* *If I can do it, you can do it too*
* Embed *watercolor map* from Stamen, like in [this codepen](http://codepen.io/fwebdesign/pen/DyAto)


### 19.09

* Presentation went really well, let's see if people choose any of the Google Trends..
* I think getting people to plan their comic is a good idea in principle, and it may be worth spending 5 minutes doing that before we dig into code. Perhaps as a rough sketch? Also I should show examples of what a Web comic can be.. simple pages that can be done with a bit of HTML and CSS
* To explain CSS, use **dress code** as a metaphor
* `position:relative` and `position:absolute` is still bloody tricky, let's re-introduce the boilerplate style
* [x] Re-order the *spot the difference* examples so that we have all HTML ones first, then CSS
* [ ] Can we use `normalize.css`, would it help? Or maybe create a sort of normalize boilerplate and link to it
* [ ] Today we make a comic, but think of what you could do **after**? Eg create a blog for yourself or a friend, make a webpage for your music band, etc. and mention [Dash](https://dash.generalassemb.ly/)
* [x] Make the `max-width: 600px` and `margin:auto` earlier, maybe right after the `background`
* [x] Need to get people **used** to `id` and `class`, do it at least 3 times, before we introduce new properties


### 24.09

* [x] **What is...**, **What if...**, **Hot to...** instead of sketching the comic
* [ ] **Boilerplate** on GitHub should be possible, but not as raw, maybe grab the link from the Pages branch?
* [x] Give all the speech bubbles `id` names before we style them (works well)
* [x] Introduce `width` and `height` before they hack away
* [ ] Show how to **embed a video** in the morning
* [ ] Show how to **embed a map** in the morning (people are uninspired otherwise)
 

### 25.09

* Use [IFTT](https://ifttt.com) as an example of **programming logic**?

### 26.09

* [x] Need to make the **presentation shorter** (20 minutes, about 1 minute per slide). Speed up, don't spend much time asking questions.
* [x] Typing in the **skeleton** from scratch worked well, less errors later on.
* **What if** etc. also seemed to work well, people picked more interesting topics.
* [x] Let's do the `position` style after fonts, after lunch break.
* Not sure if `element.style` is a good way to introduce CSS 
* [x] We need a **slide** for HTML and CSS
* [ ] How to get people more **excited** about the potential of Web-making? We should tell them that by the end of the day they'll have made **their first very own web page**, and once you made a page you can take that knowledge further to make a website, customise your blog, get paid to make websites for someone else, code an app.. it's the **start of a journey**. 
* [ ] Maybe the initial slides about **spotting differences** are putting people off? Need to make them more fun, turn them into a competitive activity between two teams? Or note down the differences and then ask them how many they've spotted?
* [x] They don't want to make comics, they want to make **apps**!

### 27.09

* [x] Let's try and **make an app** then. It can be a simple *Help me decide* one, where you type in two options in a stylish `form` and there's a bit of **JS** code that picks one randomly and then presents it to you in a glorified, *You should {option 1}* way, similar to the [Authentic weather app](http://authenticweather.com/). It can easily be extended to become a *paper-scissors-stone game*. It should have *social sharing* options once you've got your response.

#### JSBin or CodePen?

##### CodePen

	+ Comes with SCSS
	+ Comes with reset.css and normalize.css
	+ Supports HAML and SLIM
	- Hides <head>, is that good or  bad?
	+ Can text yourself a link to your pens!
	- Full URL comes with a CodePen footer
	+ Seems more of a community (profiles, blogs, collections, bookmarks)
	+ Embed jQuery, and add any other libraries you may want/need
	- Doesn't save automatically
	
##### JSBin

	- No support for HAML or SLIM (but JADE)
	+ Shows you the <head> 
	+ It's more transparent when you drop in a library (adds it to the <head>)
	+ CONSOLE tab to noodle
	
	
### 01.10

#### Presentation

* *How does it wwwork?* "Just tell us" one said
* They like  *WWWtf*
* *Database* joke could work, but I have to exaggerate it a bit
* **Open what?** slide needs a bit of a verbal transition and intro

#### APPtivity

* Showed the finished app before getting the HTML *shopping list*
* Elements first, attributes later (starting with `placeholder`, then `type`, `name` and `for`)
* *Democracy*: when we finished the HTML part, I asked students to **choose** if they wanted to style the app first, or make it work. Majority: make it work. OK, but keep in mind that styling is going to be easier than make it work. Hands up, still the majority of people want to go for the hard task first :)
* *Democracy* is nice but maybe we want to do some styling before we dig into JS. people should respond better to an app that looks good, rather than one that looks shitty.
* **JS doodling** without calculator. Started with `hello / "hello"`, moved on to `alert()` and `prompt()`, then variables
* Showed the **Web Inspector** and *hacked* Facebook before meeting the **Console**. Changing the the text to *Facebook **doesn't** help you connect..* sparked amusement (more than changing the `background`)	
* [x] As a first JS task, after the `console.log()` we could do `p.hide()` and then `p.fadeIn()` inside the `onSubmitForm` function? The idea is to give people some quick win, otherwise they'll get bored before they can see anything appearing on screen!
* [ ] As a second task, we could build a `makeDecision` or so function. Explain that we could put some complex logic to it, but for now we're just going to spit a random number.
* Robot activity worked well :)
* [x] How do we introduce *concatenation*? With `console.log("option1 is " + option1)`.
* [x] Need to get default values to the inputs to avoid typing in all the time
* [x] Tweet and FB buttons we can do later
* [x] CSS or sass? Doesn't work well with Google Fonts, so let's stick to CSS
* [x] Easy CSS stuff like color and background first
* [ ] How to make the `p#message` style easier / less lines?
* [x] `display:none` is an easy one to show

### 02.10

#### Presentation

* [x] Show **reveal.js** instead (or tegether with) jQuery in the **Open what?** slide

#### APPtivity

* Used **standard HTML** (not SLIM), as people findcode to copy-paste elsewhere in this format
* Used **standard CSS** (not SASS, there's no need for it for such a small thing)
* [x] Tiny bit of CSS to center the `h1` and hide the `p`, then dig into JS
* [x] Quick win with JS is `p.fadeIn()`, then wrap it inside `form.on("submit", doSomething)`
* [x] `doSomething` is not defined, let them experience the **error** (maybe let them experience also `jQuery is undefined`?)
* **Console**: got asked again *What's the purpose of this?* when showing `Math.random()`. Is it the maths that put people off, or the whole *getting familiar with the console* part? 
* [ ] Keep **console noodling** to the minimum. Define a set of things/concepts to show before we go back to the app.
* People understand that it's **useful to log stuff** in the console, because with JS, unlike HTML and CSS, we can't see immediately whether it works or not.

### 03.10

#### Presentation

* Slow start, mumbled the first slide but then picked myself up. Need to practice the first slide really well, cause it's the hardest moment (you're sleepy, they're sleepy) and it doesn't make a good impression if you sound like a cranky engine starting up.

#### APPtivity

* Use **standard HTML**, people get it :)
* [x] Maybe we don't need `#message`?
* Explaining `form` by showing Google search works well
* People don't get the difference between `placeholder` and `value` unless we make it explicit	
* Before jumping into JS, do a bit of CSS. Quick wins like 
	* `text-align: center;` for `h1`
	* `font-size`, `padding`, `color` and `background-color` for `button`
* Show [Kuler](https://kuler.adobe.com/create/color-wheel/) to pick colours and introduce #hex values
* We got all the JS done before lunch! But how much did they actually understand? I think `variables` are still not clear
* [ ] People struggle with `getRandom(min,max)` and `getRandom(0,1)`.. how to explain that?
* [ ] People struggle with the idea of replacing `option2` with `choice`

#### POP

* [ ] People get the idea of coding a robot, however they start by giving it very specific instructions (eg: walk 3 steps, turn 30 degrees, walk 2 steps). We can build an understading of **abstract functions** from there
