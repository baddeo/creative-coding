# APPtivity

## Let's code

1. Find **CodePen**
* Sign up
* Create new pen
* Remember to **save** your pen(s) `⌘ + S`

## Structure

1. Set up the HTML box: enable [SLIM](http://slim-lang.com/) and hide the JS and CSS boxes
* Write all the content of our app 
* `h1` (let's keep this because it'll be useful for Google Fonts)
* `form`
* `input` (Make sure you add `name` attributes!)
*  `button`
* `p#message`
* `a` links to share on TW and FB (kind of *optional*, but rather important to leanr how to make hyperlinks, and how to use `class` with eg: `a.link`)
* **Compiled preview**

##### OPTIONAL 



## Behaviour

1. Introduce `console.log`
* Include **jQuery** (explain *libraries*)
* Define **variables**
	
	    form = jQuery('form'); // the form
	    options = []; // an empty array
		chosenOption
		chosenValue
	
* Introduce **comments**
* **Noodling?** 
* Introduce **arrays**
* Introduce **functions**
* Let's *google* `jquery input values to array` (will bring up the [jQuery.serializeArray()](api.jquery.com/serializearray) method)
* Let's *google* `JS function to get random number` (one of the first results will be from [StackOverflow](http://stackoverflow.com/questions/1527803/), good chance to introduce SO and pick the function we need)
* Isolate the **value** that corresponds to the random option
  
      chosenValue = options[chosenOption].value
      
  This will be tricky I reckon.
* Display the **message** (string **concatenation**)
* Bonus: make the message *motivational* with `f*****`  


#### Later

1. Make `p#message` fade in and fade out on click
* Give the social buttons some behaviour



## Style

1. Setup: `SCSS` (or `SASS`?) with `normalize.css`
* `p#message`

        p#message
		{
		  font-size: 50px;
		  font-weight: bold;
		  text-align: center;
		  position: absolute;
		  width: 100%;
		  height: 100%;
		  background: rgba(173, 255, 47, 0.9); // greenyellow
		  top: 0;
		  margin: 0;
		  padding-top: 20%;
		
		  display: none;
		}
* `h1` centred
* **TODO** Loads of styling here...
* `-webkit-appearance: none;`
* [Font-Awesome](http://fortawesome.github.io/Font-Awesome/) for social icons?



## What next?

1. Add the app to your phone's **home screen**
 
         <link rel="apple-touch-icon" href="http://i.imgur.com/ln9kdl3.png">
 
* Hook it to an **API** (eg: weather, maps, videos, music, [unistats](http://unistats.direct.gov.uk/)...)
* Turn it into a **paper-scissors-stone** game


### Debug

* Form submit on `Enter` only with one `input`, if you have 2+ then you need a `submit` input/button



http://codepen.io/baddeo/full/jsICq/
