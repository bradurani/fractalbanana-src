---
layout: post
title: "Reviews of 5 JavaScript Books"
date: 2014-04-23 06:06:30 -0500
comments: true
categories: JavaScript, Book Reviews, Software
---



__TL;DR:__ Start with [The Good Parts](http://www.amazon.com/JavaScript-Good-Parts-Douglas-Crockford/dp/0596517742/), then read [JavaScript Patterns](http://www.amazon.com/JavaScript-Patterns-Stoyan-Stefanov/dp/0596806752/) if you’re hungry for more. Read [Functional JavaScript](http://www.amazon.com/Functional-JavaScript-Introducing-Programming-Underscore-js/dp/1449360726/) when you’re ready to have your mind blown and learn a new way to program. [Testable JavaScript](http://www.amazon.com/Testable-JavaScript-Mark-Ethan-Trostler/dp/1449323391/) and [JavaScript Testing with Jasmine](http://www.amazon.com/JavaScript-Testing-Jasmine-Behavior-Driven-Development/dp/1449356370/) can be skipped provided you know it’s a great idea to use event hubs and write unit tests.

18 years after I wrote my first line of JavaScript (Netscape 2.0 for Macintosh was released in March of 1996), I decided it was time to catch up on the latest best practices and fill in the gaps of my dated understanding of JavaScript. I guess I’m late to the JavaScript renaissance, but it only took 5 books to bring me up to speed. The result? A very slick open source micro-framework called Ranger (http://www.github.com/bradurani/ranger) that I’ll blog about as soon as I’ve documented it. Here’s how I got there

## Review: [JavaScript the Good Parts](http://www.amazon.com/JavaScript-Good-Parts-Douglas-Crockford/dp/0596517742/) - Douglas Crockford ##

The best programming books are the ones that show you examples of what NOT to do. This is just such a book. In fact, it could just as easily be called “JavaScript the Bad Parts”, but I suppose it wouldn’t sell as well. It’s a classic, and it’s the first book you should read when you’re ready to admit that loose collections of barely organized jQuery do not an application organize.  
It’s opinionated - to a fault in fact. And while it’s heavy on language mechanics with nary a hint on how to put them into practice, that’s no excuse for skipping it. It’s barely 100 pages, and it sets the stage for everything that comes after it. JavaScript is a quirky language and its proclivities are easy to forget. You have to read about them several times and experiment if you’re going to remember them. Crockford’s book is the perfect first exposure, plus you can name drop him during any job interview and get instant brownie points.  
Read it, digest it, read it again. Try out his linter, JSLint, then ditch it for the less opinionated JSHint. Only when you’re fully steeped in the bad parts, should you move on to something more imminently practical. It’s also worth checking out his video on the subject [here](https://www.youtube.com/watch?v=hQVTIJBZook), but watching it doesn’t excuse you from reading the book.

## Review: [Testable JavaScript](http://www.amazon.com/Testable-JavaScript-Mark-Ethan-Trostler/dp/1449323391/) - Mark Ethan Trostler ##

I had high hopes for this book but most of it wasn’t useful to me. the first few chapters, however, were worth the price of admission. Chapter 1 is the perfect exposition and eminently quotable :  
“Your ideas are unique, your code is not”  
“Testable JavaScript is your gateway to sanity”  
“Unit tests are a developer’s first line of defense”  
But it’s chapter 2 where the value of this books lies. Here we study command / query separation, function decomposition, and scoping for testability. There are great discussions of cyclomatic complexity, fan in and fan out, and a complete Linnean breakdown of the genera of coupling. Most impressive indeed, especially since we also get a full dose of dependency injection (one of my favorite subjects) and a comprehensive look at documentation tools.  
Chapter 3 makes a convincing case for event-based architecture. So convincing, in fact, that I now use event-based architectures for everything I build with JavaScript (and I’m not talking about click events and other jQuery gimmies, I was already using those). The event hub example (the most important pattern in JavaScript architecture?), is a server-side example for node.js, but the point is still made, even if you only write JS for browsers.  
Chapter 4 mixes great advice about unit-testing, with annoying examples using the YUI framework, which I don’t use ([Jasmine](http://jasmine.github.io/) is better). It has a great breakdown of mocks, stubs and spies, then veers off into tools such as PhantomJS (a headless browser) and Selenium (a functional testing tool). Pick and choose here, there are useful bits between the tool focused parts.  
The rest of the book was useful, or maybe useless. I’m not sure, I didn’t read it. It’s about tools for code coverage and load testing and automation and things only NodeJS developers care about. Read it if you want, but it’s probably already out-of-date. The first 3.5 chapters are very good though.

## Review: [JavaScript Patterns](http://www.amazon.com/JavaScript-Patterns-Stoyan-Stefanov/dp/0596806752/) - Stoyan Stefanov ##

This book picks up where “The Good Parts” leaves off. Actually, it starts by repeating everything from “The Good Parts”, which is great, because you forgot those things, and need to see them again. What comes after is what’s really useful: page after of page of practical, usable design patterns that you can use in your own applications. You get 5 versions of inheritance, a panoply of object construction variations, and an almost complete rehash of the [Gang of Four classics](http://www.amazon.com/Design-Patterns-Elements-Reusable-Object-Oriented/dp/0201633612/). Best though, are the module, namespace and sandbox patterns, which have spawned many micro-frameworks.   
This is solid, usable stuff. Even if you don’t write your own framework (this book gives you the pieces), these lessons help you identify patterns you see in the wild, and the first step to becoming an application architect is identifying patterns by name. If you don’t have time to read the whole book (shame on you), there’s a nice blog post [here](http://addyosmani.com/largescalejavascript/) that summerizes many of the more useful patterns.

## Review: [JavaScript Testing with Jasmine](http://www.amazon.com/JavaScript-Testing-Jasmine-Behavior-Driven-Development/dp/1449356370/) - Evan Hahn
Jasmine is stellar  
This book is out of date now  
Skip it and read [docs](http://jasmine.github.io/)

## Review: [Functional JavaScript](http://www.amazon.com/Functional-JavaScript-Introducing-Programming-Underscore-js/dp/1449360726/) - Michael Fogus ##

Ok LISPers, Scala Jockeys and Clojurites, you’ve got the jump on me here. I mean I know about lambdas, map, reduce and filter, but those are tools for writing concise functions, not architectures for entire applications... or so I thought. Let me back up. I’ve known about functional programming for many years, and being a former C# dev, I know that lambdas are a way of life. However I never knew exactly how to translate those concepts to architectural patterns. I’d been prosthelytizing the trees but missing the forest.  
Functional programming is about composing functions to create pipelines for data transformation, and if you haven’t read a book like this, or practiced it yourself, it’s not easily intuited. It’s functions instead of loops, functions instead of ifs, functions returning functions and taking functions as arguments. It’s not just about pulling punchy one-liners like you Rubyists gloat about. Functional programming is a lifestyle, a higher-order of being where everything’s a function and inheritance only marginally useful.  
That JavaScript is functional at all is a small miracle. It happened sometime between 2:00 am and 4:00 am in February of 1996 - when Brendan Eich was blessed with an ephiphany, imparted by angels like an annunciation on a [gothic triptych](http://en.wikipedia.org/wiki/M%C3%A9rode_Altarpiece): functions should be first class objects. He took the road less-traveled - a sharp turn off the highway towards Java-like languages that the world was hell-bent on following at the time. JavaScript was not a complete failure, having inherited just enough LISP to make it really useful.  
The build up is slow. Ravel’s Bolero, but it’s not a sex scene. We hear readable, reusable code composed of tiny simple functions - short sharp drum beats that build to form a symphony. It’s complexity simplified to the simplest it can be, and not a drop simpler.  
And what’s this I finally understand? Monads! They’re not burritos, nor train cars, nor spacesuits nor any other obfuscating metaphor. They’re abstractions used to augment primitives with additional processing rules as they travel through data transformation pipelines. “You had the power all along, my dear”, said the good witch to Dorothy, “and you realized it on page 185”.   
There is life after inheritance. There’s more than OO. Now pass me that function and I’ll give you one back. Recurse until you catch the final burrito, the final train car, the final space suit. Peal back the foil and behold the result. The new JavaScript is functional. Now where do I learn more about Scala?