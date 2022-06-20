**pputt** is a scorecard application for PPutt.

Its primary accecss is via this URL, which we expect to most often be accessed by QR code:

[pputt.app](http://pputt.app)

![qr-code-styling](https://user-images.githubusercontent.com/2374730/174653655-eb081435-b9a7-40c8-9d12-971ee1dc2987.png)



(In a business context, we plan for this QR code to be posted at the entry site of the course in question. That's where the majority of our users will come from.)

- [ ] Add mockup sticker/share sheet(s)

We expect most users to interact with the application through a web browser. For regular users, we provide a PWA interface that eliminates unnecessary browser UI items for a more focused, fool-proof experience. (We don't promise improved feature functionality in the PWA, because we want to focus on making the experience for the first-time user as good as possible.)

The primary pages in the interface are:
1. Scorecard
2. Settings
3. Course info (incl. rules)

These are ordered intentionally, in terms of software development—

We first need a scorecard that is functional at an individual, anonymous level;
then we'll build the concept of associating specific user data to each Scorecard;
then we build the concept of tracking what Course the Scorecard is associated with. 

—and from a marketing/growth planning perspective:

We're starting by creating an anonymous, easy to use tool that can be developed cheaply and offered free to grow the platform. 
- [ ] Risk check: Est. marginal cost of operating this application at scale 100, 1k, 10k MAU
Once we demonstrate demand for this type of tool, we can start selling customization to golf courses for their Course info page. (It's a bit of a Yelp-dick move, described this way, so I think we have to be principled about this.) 

**This is the potential monetization.**

> PPutt.app, to [Interbay Golf Center]: "We have 1k users per month using our app to keep track of scores on your course. For $5/mo, you can customize the landing page they get from this QR code, and we'll default-suggest that they report their scores to your system so you can track them in your database—e.g. for league-scoring, running company/event tournaments quickly/easily."

- [ ] White Paper: Running a PPutt tournament on the PPutt platform. ("It's Google Sheets all the way down.")

# Scorecard

The current version of our scorecard app should be considered the prototype:
[pputt.app](http://pputt.app)

- [ ] It's currently served from a pitcherputt.com TLD; we'll change that

# Settings
We'll start by using browser cookies to store basic info about users. This works in the first-time and PWA use cases (as demonstrated by Dunbar).

1. Player name
2. Auto-submit scores to user-defined GSheet "database"

# Course info

1. A default set of rules for putt putt everywhere.
2. A statically-served page for the PPutt rules to be used at Interbay, esp. for our tournaments.
