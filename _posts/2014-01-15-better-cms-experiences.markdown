---
layout: default
title: "We need to deliver better CMS experiences."
date: 2014-01-15 23:11:11
excerpt: "“I just don’t understand how to use my website’s CMS.” This, or some variation of it, is a gripe I hear all too often from prospective clients. I’ve actually had clients tell me they’ve never —not since day one— managed to feel confident using their website’s CMS. What’s up with that?"
---

We strive to deliver the best experiences for our clients’ users. Websites are snappy and responsive, content is accessible and presented beautifully, launch goes without a hitch. The project is a success… Eventually, our client gets their hands on it and they have no idea what they’re doing, so they improvise: They dump content where it doesn’t belong, spend countless hours figuring out how the formatting on the editor will translate to the front-end, and finally come up with a list of little tricks that make the site behave in a certain way that is contrary to our intentions, but which they think somehow enhances the content. And that’s when the site loses its luster.

More times than not, that’s our fault.

## WYSInotWYG
WYSIWYG editors are pretty powerful these days. They can deliver pristine markup, offer clickable tools to add classes and styles, limit the HTML elements people can use, provide templates with pre-defined and pre-populated blocks of content, and —most importantly— provide an accurate, live preview of what the content will look like on the front-end. In my experience, however, many developers deliver WYSIWYG editors with stock stylesheets bearing no resemblance to the front-end, unrestricted access to any number of style modifications (often —if not always— applied with the less-than-desirable `<span style="[…]"></span>` or similar), and no assistive tools to help structure content in ways that comply with the styles and tone set forth by the design.

If we expect clients to take good care of the websites we design for them, we must provide them with the right tools for the job, and a properly configured WYSIWYG editor goes a long way to help get that job done. Look into what editor your CMS comes with out of the box. It may be one of several popular editors out there, or it may be custom made for your CMS. What ever the case may be, learn how to configure it to control your client’s experience with it:

1. Change its stylesheet to use the same styles you already defined for the front-end. Usually, this can be done by copying the relevant styles and adding the parent selector used by the editor to contain its markup. It sounds scarier than it actually is.
2. Take the time to define which tools will help your client communicate properly and within the website’s styles, and remove the tools that will not. It’s hardly ever a good idea to let a user choose any color they want for type; paragraph alignment is another great example. By removing these tools, we provide guidance and allow clients to focus on their content and not how cute and fun they can make the text look. The same goes for element types; if you know your client won’t be using `<pre>`s, remove that option.
3. If your front-end design calls for certain layout patterns (captioned images, for example, or any other specific combination of elements that together form a unified block of content, like an attributed `<blockquote>` with a `<cite>` element), use editor templates. For example, [CK Editor’s templates feature](http://ckeditor.com/about/features#user-rich-content) allows you to pre-define blocks of HTML with placeholder content, which the user can insert with a simple click. All they have to do then is select and replace the placeholders, and voilà!

Properly configured WYSIWYG editors play a huge role in making our clients’ lives easier because it allows them to follow design guidelines without much fuss. They also allow us to go beyond designing what a website looks like today, by ensuring visually, semantically and stylistically consistent client-generated updates tomorrow. If we go the extra mile on only one thing, let it be this.

## Our solutions are often prescriptive.
There’s a saying about how everything’s a nail to the guy holding a hammer, or something to that effect. Let’s not be the guy holding a hammer.

Sometimes (most times) a CMS’s default UI is just not good enough. Maybe it expects users to know too much, or it treats all content like the same kind of content. Maybe it organizes content fields in the manner in which they were created or loaded via plugins, without concern for how they relate to the front-end or what order makes more sense for the creation process. Whatever it is, there’s a good chance that the default behavior of your favorite CMS is not gonna cut it. Not because there is something inherently wrong with it, but because it was not created with _this website_ and _this client_ and _this content_ in mind.

As much as we can, we should build an interface for the CMS. This UI should be crafted with our client’s needs and abilities firmly in mind. A content creation form that makes every possible setting available, even the ones we know our client will use maybe 10% of the time and the ones that don’t really apply to this category, section, or channel but are there because they’re needed elsewhere, only serves to confuse and overwhelm the user. We can do better than that.

I’m not advocating for the creation of bespoke CMS solutions for each project. But any CMS worth its salt should provide some degree of control over the back-end user’s experience, allowing you to establish common patterns and conventions that help guide the content creation and maintenance process, and avoid confusion created by overwhelming amounts of (often irrelevant) options, settings and fields. At the very least, we should:

1. Compartmentalize and set aside the settings and fields that will be seldomly used. These should be accessible, just not front and center. Ideally, they should be hidden under a separate tab or a collapsed fieldset.
2. Hide the settings and fields that are there because they belong to a different category, section or channel of content. If it’s irrelevant to this specific entry, the client shouldn’t see or have access to it.
3. Create content creation forms for specific types of content. If one of the content types is Staff Members, for example, the form should be reflective of the needs of this type of entry (e.g. portrait, position, bio, projects they’ve worked on); it shouldn’t look like the form for publishing a news article.
4. Where ever possible, use drop-down menus, multi-select menus, searches and other UI elements to select featured or related content. This keeps the client from fudging up a link and saves them from having to write (and fudge up) content twice. It also allows you to control which categories or types of content can be highlighted or featured on a home page carrousel (for example), as well as do nifty things like setting rules to determine whether something shows up (e.g. if expired, don’t show content). Triple win!

## Post-launch support as an add-on.
I’ve met with prospective clients whose previous developers handed a website off with literally not a single minute of training. Just an email saying _”Here are your login credentials. Great doing business with you!”_ Awesome job there, bub. When asking for support or at least an introduction to their CMS, the client is presented with an estimate for a support contract. **Stellar job there, bub.**

Of course, proper training and post-launch support costs money. I wouldn’t suggest we need to be giving away our time and effort. Yet these costs should be factored in from the beginning, itemized in our estimates and described in our proposals, so the client knows that (1) they won’t be left in the dark post-launch, and (2) they won’t be surprised with added cost. I’d wager that very few cients would choose to do without training and support just to save a bit of cash, and those who do at least _know_ they won’t be getting it.

## We don’t let clients in on the _why_s and _why not_s until the very end.
Mid-project presentations need to be about more than just getting client feedback on what their site looks like and how it behaves under certain circumstances. We need to get them on-board with us regarding what the site _is_ and, more importantly, what the site _is not_. Early discussions about where different types of content should go, what the function of each section is, and the value of using the appropriate spaces for each type of content will go a long way towards establishing content publishing guidelines. Granted: some clients will still stray from these guidelines. In those cases, those post-launch support calls and training sessions I mentioned above provide plenty of opportunity to go over them again.

---

With a good CMS experience, proper training and follow-up, and making sure a client understands the purpose of their site, we inform and empower them. And that’s a good thing, because informed and empowered clients do two really awesome things:

1. **They don’t bug us with the little things.** They’ve been trained, they understand the CMS, they feel secure in their abilities. We needn’t bother with everyday content maintenance tasks. They got this!
2. **The come back to us for the big things.** Those big challenges are the ones we live for, and their long-term satisfaction makes their decision to hire us again for future projects a no-brainer. Doubleplusgood!

Building better CMS experiences for our clients is simply good business.