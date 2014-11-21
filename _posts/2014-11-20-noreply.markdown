---
layout: post
title: "On a support request, it helps to be helpful"
date: 2014-11-21 09:30:00
excerpt: "By the time a user seeks help, they’ve likely already had a negative experience, to some degree. It’s important, then, that the process of requesting support be easy, predictable, and without friction, lest we turn a customer’s mild annoyance into outright&nbsp;frustration. As usual when crafting a useful user experience, empathy is key."
image: "http://media.giphy.com/media/11M1k4fIwVqPF6/giphy.gif"
image-caption: 'GIF: Jim Carrey furiously answers an endless stream of what one might consider support requests in Bruce Almighty (2003). Bear with me here.'
comments: false
---
I’m perusing a popular creative content platform. I need graphic elements to complement a design project, and this platform has helped me find appropriate content in the past, from typefaces and textures, to hand-drawn imagery. Once again, I find a couple of pieces that are a perfect fit for my project, so decide to go ahead and make a purchase.

When I try to log in, I get an error saying my username and password do not match. This is odd, because I use a password manager to generate and store passwords. I don’t give it much thought, though, and click the ever-faithful _password reset_ link. That part is typical enough; wait for email, click on link, generate new password, submit form, save the generated password to the password manager database. But then I get the same error when I try to log in with the new credentials. Rinse, repeat; same outcome. It was time for a support request, a.k.a. “the worse time to give customers a hard time.”

{.callout} And that’s how my first ever negative experience with this previously trouble-free provider begun.

I looked at the masthead and saw no _Help_ link, button or even mention. No _About_ link to speak of, for that matter. I did notice a _Community_ link with a reverse caret beside it indicating a dropdown menu, so I hover over that to find a bunch of community-related links. While none of them seemed _Help_-related, I did notice that each of them linked to a simple, predictable, homonymous subdirectory. That is: the _Blog_ link pointed to `/blog`, and the _Discussions_ link pointed to `/discussions`. So, naturally, I tried `/help`. Noooope. There is no help to be found at `/help`.

_:sigh:_ OK, I thought, I’ll just email them.

I checked the reset password email and noticed that it came from a _hello@domain_ email. Seems friendly enough, I’ll just reply to that. After all, that email was sent as part of a password reset request that resulted from an unsuccessful login attempt; surely replies to this email are expected, since its contents might not resolve the issue that prompted it int he first place. Alas, my email was met with a reply indicating that delivery to _noreply@domain_ failed permanently. Wait, what? _noreply_? Well, that was silly of me, why would I send an email to that address? I thought I had replied to an email that came from a _hello_ address; I must be going mad. (Hey, it’s been a hell of a year so far, it’s entirely plausible that I’m losing my mind right now.)

---

_Quick parentheses here, because this is pretty amusing:_

Turns out that the password reset email I had received did have a _hello_ address in its From field, but it also had a _noreply_ address in a Reply-To field. Now, putting aside the absurdity of noreply email addresses for a moment (and they _are_ absurd), I must ask: what is the point of using a noreply address if you’re going to hide it away in a Reply-To field? After all, the point of a noreply address (as shitty a point as it may be), is to tell the user not to reply to this email _(or, more accurately, to embed a picture of its own shitty futility in its very own address)_. A message like that should be prominently displayed, not obfuscated.

But then, if you’re going to go through the trouble of setting a Reply-To field, why not set it to something useful like _support@domain_? That’s a much more thoughtful use of the Reply-To field. It allows you to keep the friendly _hello@domain_ address in the From field while directing a customer’s replies to the appropriate channel. All without breaking the behavior they expect when replying to an email.

---

So I go back to the website, frustrated, and run a search for the word _help_ on the page. That’s when I find a _Help Center_ link buried in the site’s footer (ever the knick knack drawer of orphaned links on the internet), under a _Community_ header, no less. This link points to `/hc/en-us`, a subdirectory I never would have thought to try. I used the form on that page to submit my support request and added a note about my experience with the `hello`/`noreply` email, which I hope they take to heart. (I also mentioned the lack of a prominent Help link or a useful help page at `/help`. I try to be helpful _and_ thorough in my whining.)

I don’t think this’ll be much more of a problem. Now that I seem to have gotten through to support staff, it’s reasonable to expect this super boring issue to get resolved relatively soon. But the experience has taught me a valuable user experience lesson.

A thoughtless approach to the help request experience can go a long way towards turning a mild annoyance into a frustrating experience that can easily erode confidence. A little empathy could have turned this run-of-the-mill support request into a pleasant experience that reinforced my trust in the company, and that’d have been a significant win.
