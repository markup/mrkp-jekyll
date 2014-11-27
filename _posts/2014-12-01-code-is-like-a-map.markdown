---
layout: post
title: "Code is a lot like a map."
date: 2014-12-01 09:00:00
excerpt: "We should concern ourselves not only with how efficient our code is, but also how legible. Much like a cartographer’s concern is how a map is to be read, and less so how it’s printed."
image: "/images/blog/bacons-london-1890.jpg"
image-caption: 'Map: Bacon’s New Map of London, Divided into Half Mile Squares & Circles. This work is in the public domain. <a href="http://bit.ly/1Ftoe7A">Wikimedia</a>'
comments: false
---
> “As a designer, hell, as ANY type of craftsman, you are responsible for what you help to put in the world.” <cite>—[Mike Monteiro](http://muledesign.com/2011/02/how-to-pick-the-right-clients/)</cite>
 
---

While working on my [bustime node module](https://www.npmjs.org/package/bustime "First ever node module, FTW!"), I decided to try out [Code Climate](https://codeclimate.com/dashboard) as part of an effort to be more mindful the quality of the work I put out. Code Climate can integrate a test suite into their analysis, but I’m not using tests yet (baby steps, don’t judge!). The reason I signed up is that they offer code analysis going by their [ABC Metric](http://docs.codeclimate.com/article/148-glossary-abc-metric).

The first evaluation gave every file in the project an **A**, except for one file: an object validation submodule which Code Climate gave a scathing **D**. Ouch! Upon reviewing their analysis I learned that the big issue was “method complexity”, but I saw no way to further simplify the code. _It is what it is_, I thought. _I couldn’t possibly make it more straightforward._

After mulling it over, researching the problem on [SourceMaking](http://sourcemaking.com/refactoring/long-method), emailing Code Climate support for guidance and even [tweeting about it](https://twitter.com/agarzola/status/537636431619817472) (admittedly in frustration), I found a solution to my conundrum and learned a valuable lesson in the process.

{.callout} The problem was not that my code wasn’t efficient, but rather that it was too efficient at the expense of legibility.

Where I was originally loading multiple external methods as needed in each local method, I am now building a separate object loaded with each of the external methods embeded, then referencing that local object in my methods. What once looked like this: `rt: Joi.alternatives().try(Joi.string(),Joi.number()).required()` (indicating this property’s value must be a string or a number and is required), now looks like this: `rt: valid.stringOrNumberRequired`.

It’s like my methods were a map and, in my pursuit of efficiency, I didn’t include a legend. A legendless map, with little labels for every different type of landmark or terrain, may _sound_ straightforward (after all, everything is explicitly labeled), but it ultimately makes the map difficult to read. By adding a single layer of logical complexity to my submodule, I removed several layers of cognitive complexity. It’s not unlike a legend adds a layer of visual complexity to a map yet reduces cognitive load and helps better convey meaningful information.

My takeaway is that, in addition to being efficient, code needs to also be easy to read. After all, the idea is not only for other developers to use our work, but to fork, modify, improve, learn from and share it. To that end, our code should err on the side of legibility.
