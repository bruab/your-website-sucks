---
layout: post
title: ... because your form validation tries too hard
---

The whole point of your website is to get me to fill out a form.

You want me to enter my credit card details and shipping address for a purchase. Or you need me to submit my name and email to set up a sales call. Or maybe you're hoping I'll create a username and password to use your app.

You want me to fill out a form, so once I decide to do so, _do not get in my way_.

In particular, don't reject what I type into the form when it's ... completely valid.

Like this:

[![screenshot of a form with error: "offensive language discovered in the last name field" - last name is wiener](/assets/images/natalie-wiener-form-validation.jpeg)](https://twitter.com/natalieweiner/status/1034533245839450113)

or this:

[![screenshot of a form with error: "invalid last name" - last name is O'Hearn](/assets/images/brint-ohearn-form-validation.jpeg)](https://twitter.com/brintly/status/999322836048187394)

Be careful about what form fields you set as "required" - I recently made a purchase on a site that wouldn't let me enter my shipping address without providing an apartment number:

![screenshot of "shipping address" form with error - "Enter an apartment, suite, etc."](/assets/images/error-apartment-required.png)

(I don't live in an apartment, so I just typed "..." into this field.)

And as much as you might love error messages, try to display just one at a time:

![screenshot of password input field error messages - illegible because there are two messages overlapping](/assets/images/overlapping-error-messages.png)

Adding frustration to this crucial step is a great way to make visitors reconsider their decision, and potentially abandon your site _right before converting_.

## Here's how to fix it

Honestly, I'm not sure how some of the above even came into being - so I'll start by saying: don't implement your own proprietary form validation algorithm.

Don't make up rules about how long someone's name should be.

Don't make a list of characters or words that aren't allowed to appear in a name. Just ... don't. Use an existing platform, plugin, or library.

Follow that advice, and you should be fine.

BUT if you have access to a developer, and you want to make sure you're not losing conversions to over-eager error messages, you can set up a system for detecting and correcting them.

It's possible to send [form errors as Events to Google Analytics](https://www.analyticsmania.com/post/tracking-errors-with-google-tag-manager/#form-errors) - do this, and review them every couple of weeks to make sure your validation isn't overdoing it.

While you're at it, add a session recording tool like Hotjar or Mouseflow, and have your developer flag sessions that contain form errors. 

That way you can watch replays of frustrating form interactions on your site - this agonizing experience will motivate you to fix what's wrong, guaranteed.


