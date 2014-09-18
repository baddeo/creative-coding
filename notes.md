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

 
