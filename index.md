> This is my transcripted version of SmashingConf presentations  
> Conference happened on 17-18 of March, 2015 in Oxford

> some shorthands to be awared of due to stenography stylistics: 

	u - you  
	ur - your  
	UR - User Research  
	RAF - Request Animation Frame

> Photos of speakers and conference moments: [See here](https://drive.google.com/folderview?id=0B0L3D_8Fib-gfjZLOXFDN2hxa3N2LUcxcURBbU9VNDRQNVdYVjVvOHpHMk9FMzdFNFBKMWs&usp=sharing)


# Smashing Conference - DAY 1

-----


## Christofer Merphy - A good writer...

"a technique for producing ideas" book

*reading*

- inspectional
- analytical
- syntopical
	- read more, multiple angles
	- form your own opinion 

re-read the book  
read through and over

*mental models*  
Charlie Monger - Google this guy!

*hammer syndrom*

> to a man with a hammer everything looks like a nail

branches of knowledge to know and read about  
creating a reacher mind

- psychology
- economincs
- heuristics
- mathematics
- pricing
- accounting
- anthropology

don't be afraid of writing

books: the craft of words

- macrocopy
- microcopy

1+1=3
1+1+1=5

together things mean more than on their own

sharing helps, so go ahead and share!

once u have a blog u think about writing and analyze  
socratical method of thinking - asking questions

> *resume:*    
> inspirational talk  
> read, read more, read now, open your mind for the new  
> write when you want to, don't wait for the right time, it will never come  
> don't forget to share your ideas and thoughts (start blog or smth.)


## Meagan Fischer - The why and how of designing for people  
## (how to be paid for your work and not be ashamed of it)

> [sproutvideo](https://sproutvideo.com/)

- 1 developer 
- 1 designer

*empathy in design*

write urself into existence in context of UI design

- understand feelings and needs
- exposure to users
- design effective solutions

constraints

- business goals
- what looks best
- what do people really want

get to know ur user!  
**it doesn't have to be hard**

- ask questions
- observe frustrations
- listen to unmet goals
- disple your assumptions

watch them use the product:

testing  
> [silverback](http://silverbackapp.com/)  
> [usertesting.com](http://www.usertesting.com/)

observation tools  
> [fullstory.com](https://www.fullstory.com/)  
> [inspectlet.com](http://www.inspectlet.com/)

good for making small changes (a/b testing?)

simple query emails result in useful data

- useful constraints
- meaningful content
- better critiques
- iterative changes

> *resume*:  
> inspirational talk / success story  
> be open to your users  
> be ready to meet their needs


## Richard Rutter - Don't give them what they want, Give them what they need

> [gov.uk](https://gov.uk)  
> Kensington and Chelsea planning department

analytics and getting information

- people searching about planning
- site search analysis and page visits
- search logs
- call center to get information

multiple topics merge into one service or content:  
Home > Service hub > sub hub > topic > page

performed user testing  
CMS issues > create design principles

success - in all other departments used the same philosophy of design

> *resume:*    
> inspirational talk / success story  
> get to know your users with every possible option   
> provide user testing, understand users' needs  
> create your design guide and stick with it for the best


## Yoav Weiss - Responsive images are here

Flexible images?

72% savings over using correct images according to resolution

1. Responsive Images Community Group --> <picture> proposal
Apple --> srcset proposal

picture vs srcset --> picture AND srcset

2. convincing browsers

> [indieGoGo](https://www.indiegogo.com/)

1st use case - retina images

	<img
	src="1x.jpg"
	srcset="2x.jpg 2x" == [source][descriptor]
	/>

2nd usecase - crop to the right view

	<picture>
		<source media="(min-width:45em)" srcset="large.jpg">
		...
		<img src="small.jpg" />
	</picture>

3rd usecase MIME type fallback

	type="image/webp" srcset="example.webp"
	type="image/vnd.ms-photo" srcset="example.jpx"

4 usecase variable width images

	<img src="panda.jpg"
		sizes="100vw" \\ close enough to most used
		srcset="panda200.jpg 200w,
				panda400.jpg 400w, ..."
	/>

precise targeting
	
	sizes="..."
	srcset="..."

"sizes" is an optimization

in total:

	picture
		source
			...
		img
			...

support:

	Chrome 38, Opera - most
	Firefix 38 (to be released) - partial
	IE (to be done) - partial
	Safari 8 - partial

feature detecting:
HTMLImageElement.srcset

[responsiveimages.org](http://responsiveimages.org/)

> *resume:*    
> techspirational talk (coined this one!)  
> use responsive images now for good  
> use picture if there are any specific resources due to design purposes 
> otherwise better use srcset


## Peter Bilak - rethinking publishing

> [worksthatwork.com](https://worksthatwork.com/)

many repetition among magazines  
advertising to content 55% to 45%  
*advertorial* = content mixed with ads

many editions converted to run online only  
tendency - getting revenue from online subscribers rather than ads  
digital version > print version > digital + print

subscription / Unsubscription happens over 1 email address  
design matters - creativity changes the world  
stop adding, think about removing approach (removing signs for traffic)

> chungking mansions | the world inside the building

community!

> *resume:*     
> inspirational talk / success story  
> re-think your publishing strategy - is it good enough to meet customers' needs?  
> ask your customers! are you ready to adapt for digital?  
> sometimes deleting rather than adding is the best way to evolve


## Natalie Yadrentseva - Visualisation that takes us beyond the numbers

people don't think about things they don't see

*visual management*

> [targetprocess](http://www.targetprocess.com/)

visual approach 

- applying techniques in daily routine
- computer visualisation

choose the beneficial angle  
how we will look at the data

- categories
- hierarchy
- time-series

structuring data

- organizing into sections
- make a model
- changes over time (future casting)
- networks and connection help to reveal bottlenecks
- analyze dependencies to understand small tasks and big goals

spatial mapping

- use hue to alarm
- use intensity to investigate

*using computer*

use templates to speed start with raw data visualisation

bad thing: dog can ruin your notes on stickers  
solution: use digital data

pros:

- learning from historical data
- common knowledge base

> *resume:*  
> somewhat observation talk  
> unfortunately in so many posible ways  
> it happens to be the most nebulous and CO talk at the SmashingConf


## Tom Giannattasio - Beyond the browser

> [macaw.co](http://macaw.co/)

*hybrid apps*

node webkit  
[nw.js](http://nwjs.io/) (powered by Intel)

	npm install nw > package.json + index.html > build

	package.json:

	toolbar: false
	chromium-args: --enable-experimental-web-platform-features

coding the app

	var gui = require nw.gui
	var nativeWindow = gui.Window.get()
	nativeWindow.close()

	-webkit-app-region: drag to move app

	// referring to the Shell
	gui.Shell.someMethod

> macaw advertisement / story goes here

features:

- observe events
- virtual DOM
- CSSOM

	document.styleSheets.cssRules
	allows to add styles
	rule.style.color = "#ff0"
	happens in 0.5ms

- virtual CSSOM 15ms vs LiveReload 220ms

> *resume:*    
> awesome techspirational presentation, better get the slides  
> hybrid apps are really great thing for non-programmers  
> with the help of node you can build powerful desktop apps


## Bruce Lawson - Is Blink the new IE6?

> [brucelawson.co.uk](http://brucelawson.co.uk)

Era of Netscape -  
problem  
no support for needed features  
then came the IE6  
everybody loved IE6

*WE* made it hard for other browsers to get to other sites

iphone coming  
danger of webkit

presto came  
started to build sites that only look good in webkit

Vendor prefixes are bad   
refuse from using prefixes  
and leaving -webkit only for experimental features  
for the good of the web

Mobile Web should just work for everyone!

Blink is making the web better  
by awsomizing mobile web

blink - is monopoly bad?  
is it a monopoly yet?

Native apps is scary thing -   
apps continue to dominate the web.  
Web apps without network don't work.

Service workers for the win!  
Invoked if you are offline.

Bookmarks on the web is useless thing,  
90% of users never used them.

Apps are the bookmarks on the mob.

> *resume:*    
> Bruce is amazing, as always  
> check out his "Service Workers" logo  
> And don't use vendor prefixes to prevent one browser only domination


# Smashing Conference - DAY 2

-----


## Mystery speaker - Chris Heilman

> used to work for Mozilla -> Microsoft now
> compares the contemporary situation to ["fintlewoodlewix"](http://en.wikipedia.org/wiki/Places_in_The_Hitchhiker%27s_Guide_to_the_Galaxy#Earth)

brutal techhy world  
I don't understand things  
this brings no fun yet

don't fight for knowledge  
find one thing and stick with it

leave people control for apps and web  
(no popups and push notifications)

web as we know it is in danger

we lost communication skills  
techno babble and geek speak

stop complaining about slow computers  
other people need simple things

build for people who are around us  
excellence through repetition  
learn things through failing

there is too much to do  
mobile histeria

> [status.modern.ie](https://status.modern.ie/)

**request features for browsers!**

web obesity  
optimize your config  
speed up your products

> [webpagetest](http://www.webpagetest.org/)

stay low and make great products for people  
do what makes you happy

> *resume:*  
> inspirational talk, lots of good points to endorse  
> stop complaining and do your best for the users, *now*  
> essentially it doesn't matter whether you use Grunt > SASS > CSS or just CSS  
> result is the king


## Zoe Gillenwater - Enhancing responsiveness with flexbox

> [booking.com](http://www.booking.com/)

flexbox solves many problems with layout  
global support 92% / 72% unprefixed

use FB as progressive enhancement  
don't use in a way it makes things look like crap

FB can make site _more_ responsive

- better use of space
- reorder content due to screen sizes

modernizr use as needed  
via classes .flexbox, .no-flexbox etc.

> margin: auto behavior  
> uses all extra space to fill

fallbacks

	display: table
	display: flex

	float: left
	position: relative
	display: flex

media queries with flexbox to enhance UI

use "order" property to control content
> only works for siblings

solution for screen readers  
to control the right HTML order

mobile only reordering:
	
	container:
		display: flex
		flex-direction: column
	item:
		order: -1

using flexbox today

- choose browsers to support
- skip '09 syntax
- setup tools with autoprefixing
- use modernizr
- choos right layout

flexbox overrides

- floats
- table-cell
- inline-block

not

- absolute positioning

> *resume:*    
> tech / tutorial presentation  
> great points of FlexBox' best parts and practicies  
> stick with slides for more accurate code 


## Lorna Mitchell - Debugging HTTP

> extensive experiene working with http

debugging stages

- denial
- frustration
- disbelief
- testing (curious)
- gotcha

seeing the problem is usually harder than finding one

developer tools  
broken search response

- headers > query
- copy as curl - everything what browser send
- change the query manually

> [curl.haxx.se](http://curl.haxx.se/)

curl cheat sheet

	-X - the verb
	-H - header to send
	-d body data
	-s silent switch
	-c / -b where to store cookies and storage
	-v show headers for req/res

postman - [getpostman.com](http://getpostman.com)  
RESTclient - [restclient](http://restclient.net/)  
Paw for Mac - [Paw](https://luckymarmot.com/paw)

> [ngrock.com](https://ngrok.com/) - expose local websites to the wider web

cool for device testing

web interface (port 4040)  
inspect resources and requests

> [charlesproxy.com](http://www.charlesproxy.com/) ($50 with trial period)

multi-platform web debugging platform

- use for debugging
- throttling
- use for proxying and develop on devices
- rewrite tool for response
- debug SSL

> [fiddler](http://www.telerik.com/fiddler) is charles free equivalent

> *resume:*    
> nice tech / observation talk  
> definitely will use ngrock in the nearest future
> also, don't give up to broken http request, it happens


## Paul Lewis - Making a silky smooth web

> works at Chrome

**page load is king**

JS is 5MB gzipped

perfomance is alot more  
service workers again - speed load from cold state

- recalculate style (matching things)
- render tree
- layout (do the boxes with widths and heights)
- painting
- compositing (trigger repainting)

> composite layers for faster perf

JS - Style - Compositing  
is the lightest sequence  
perfect for animations

*Javascript*

- badly timed scripts
- use RAF
- in case of lonng script use workers
- workers don't have DOM access
- use virtual DOM

- garbagy scripts

> [JS Memory Masterclass from Addy Osmani](http://addyosmani.com/blog/video-javascript-memory-management-masterclass/)

- use JS profiler checkbox in chrome tools

*styles*

- did i limit the scope
- are the selectors fast

*layout*

- Read then Write for the best perfomance

	var w = el.offsetWidth - cache the var
	el.width = w;

*paint*

the most painful, cause triggered by all operations  
use paint profiler to see how elements actually painted

can i reduce paint area?

- will-change: transform - modern way
- transform: translateZ(0) - retro stuff

will-change has a pixel budget  
don't overpass it

*composite*

element needs to be on its own composition layer  
pay attention to the layers system  
use profiler 

*touch and input*
scroll perf

RAIL

	response    100ms
	Animation    10ms
	Idle         50ms - time to use the workers
	Load       1000ms

Perfomance is not a unit test  
Prioritize the user needs   
[slides](https://bit.ly/rail-perf)

> *resume:*    
> cool tech presentation!  
> describes in details the pages loading process  
> and how to debug it for optimum perfomance  
> stick with page loading time, introduce the budget if needed


## Polle de Maagt - Crafting for World domination

> [KLM](https://www.klm.com/)

how could we use small changes to achieve something big  
like writing Thank you on bills results in 27% more tips for the bar host

KLM surprise campaign  
28 passengers - 1000000 reactions - 88 countries spread

another campaign  
use trained dog for retrieving lost stuff on the plane  
check operatively after flight  
view social media about people and find them  
(dog is a lie, though)  
in the past just 2 people part time browsing tweets  
70 people full-time now

implemented timer with average response time on social media

integrated payment method via social networking  
**weekly income of 80000 euros with 3500 investment**

> *resume:*    
> inspirational talk / succes story  
> work with users' and customers' social profiles to get the most of your campaign  
> can't forget the "dog frustration moment" :(


## Rachel Simpson - User research for Designers and Engineers

> UX specialist at Google

[designj.am](http://designj.am)

what we will build?

research for Swiffer  
how people wash floors  
18 homes involved    
conceptual product + user research = great product

stakeholders don't get the value of research  
talking to users is scary

why do?

- new opportunitites
- build the right thing
- fail early and often

UR is way of understanding people needs
Discover - Ideate - Design and Iterate - Evaluate - repeat

Basics

- doing better than asking
- don't interpret just observe
- ask open ended questions
- be Dr. Freud

don't

- sell ur product
- tell them HOW to use it
- make them say if they like it

Early-stage methods

Literature
	
- review all others researches
- card sorting
- cultural probes
- co-design

Prototyping tools

> [pop app](https://popapp.in/)  
great to test app ideas

> [keynotopia](http://keynotopia.com/)  
harder to get feedback

Cognitive walkthrough  
Users think:

- what is this
- do i trust you
- what u offering
- how do i get it

> [The scrollwheel](http://www.youtube.com/watch?v=fa9DLxDtPtc)

> User testing recommended book by Steve Krug  
> Rocket surgery made easy

- include others in the study
- document visually
- write a report and present it!!!

> *resume:*    
> pretty detailed guiding presenation  
> guess no one left with the idea of UR non-sense  
> should try theese apps for prototyping


## Jake Archibald - UX of Offline First

Performance matters!

> again - [webpagetest](http://www.webpagetest.org/)

does it make what it takes to load?

talky.io debugging

> splash screen is an admission for failure

- add come content
- unblock scripts

get js out of rendering path 

- lie to the users for perfomance point

unblock fonts  
[loadCSS.js](https://github.com/filamentgroup/loadCSS)

load script separately if they 20-30k and do different things  

optimising for a full cache

sometimes this happen: 

- start css js load
- css js loaded
- execute cs / js
- rendered markup content

append link child and script child via RAF

	RAF(function(){
		['css1', 'css2'].each(...)
	});

**treat the network as an enhancement**

"Lie-Fi" limbo in poor wi-fi connection

	if('serviceWorker' in navigator){
		navigator,serviceWorker.register('/sw.js');
	}

browser events  
.install --> caches.open()  
.fetch --> respond with matched cache

page loads almost instantly

unobtrusive updates - add another version of app into queue

dynamic updates  
going in background to the internet and put the version in the cache

> [isserviceworkersready](https://jakearchibald.github.io/isserviceworkerready/)

[Slides](speakerdeck.com/jaffathecake)

> *resume:*    
> great techspirational presentation  
> I wish more of such talks at the conference(s)  
> re-think your apps - in the matter of Offline-first  
> does it work fast? does it even work?  
> harness loadCSS, service workers and RAF for what suites ur needs most


-----

> Thank you for reading! Any [feedback](mailto:stewiekillsloiss@gmail.com) much appreciated.  
> 21.03.2015 | [https://github.com/XOP](https://github.com/XOP)  