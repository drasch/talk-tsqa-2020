## oneline

The concept of technical debt gets a bad name and prevents us from taking control of our universe

## abstract
Lots of organizations struggle with technical debt, both in terms of software quality and in terms of psychology. That feeling when you think part of the product, code, or testing suite isn't getting its due. That feeling that you "should" be shifting design, testing, and architecture further left in the process, but you can't figure out why it's not working.

Lots of engineers, testers, managers, and teams struggle to shift the victimization into an action plan because there's lots of misinformation about what technical debt is, when it's created, and when it's destroyed.

Most of this comes from the framing of debt as a concept. Traditionally, we hide the idea that the value of testing, code, and products can shift wildly over short periods of time. Even for stable (read sane) teams agile ENCOURAGES us to react to real information and learn from it. If we learn a product idea isn't working, we should work to evolve, change, or eliminate it. Overnight, a given suite of tests, code, or product may become technical debt. This doesn't sound like debt to me, but some sort of more sinister investment instrument.

To better wrangle technical debt we need to both learn when it's harmful and when to leverage it, and finally how to craft a backlog that doesn't leave teams feeling like they have to either pack everything in as upfront effort (such as a full automation suite) nor "convince" higher-ups that we need to "go back" and refactor, retool, or implement testing for this feature.

My talk suggests we can learn to discuss these challenges differently to make them more of a shared-solution rather than a adversarial "campaign" to convince people to invest in things.


## talk


We can think about technical debt in different ways to help us get out of the black hole and move our products into orbit with confidence.

This talk isn't going to be a bunch of really pretty slides, but an experience. I'm but a coach leading you on a hike through the forest I've visited many times. That being said, we may find fallen trees, and we will discover new things we've walked by many times and never seen.

You're going to help me, and we're all going to learn something today.

--- slide

Housekeeping

---

Code of conduct - Thank you TSQA for authoring and putting the code of conduct front and center. Just a reminder that everyone here has agreed to abide by the code and if you haven't reviewed it, you should go do so instead of listening to me.

---
Transcript available

---
Credits and citations are provided for any art, references. If something is missing, incorrect, please drop me a note.
---

I'm happy to take questions, clarifications, whenever they pop into your head. Data shows on average men will ask almost twice as many as women at an event like this, even when women make up 75% or more of the audience. Underrepresented minorities have also been shown to ask fewer questions. In keeping with the code of conduct, I'd like to encourage those quieter groups to ask your questions! For everyone else, I'd encourage you to take a pause before you ask and think to yourself whether this is a "during the talk" question or an "conversation afterward" question (or maybe a "wait and see question").

---
Agenda?

---
blank slide

---

This is a map of things we've left behind in space. Each now has to be tracked, monitored and maintained whether it's the most important satellite for predicting weather, or whether it's a plastic bottle that flew out of the space station during garbage pickup.  Currently, the cost of removing any space debris is estimated to be about the same cost as creating and launching the equipment to begin with.

Luckily, most of problem is much easier than this.

---

We talk about Technical debt a lot in the industry. Many talks are given about how to minimize it, convince management that it exists, and destroy it.

Let's do a show of hands, who has talked about technical debt in the last week....
month...
ever?

What if we add in hearing someone else (other than me) talking about it?

---
One of the main reasons we spend lots of time talking about something is because of how it makes us feel. I'd like to hear some examples of how techncial debt makes us feel?

I've provided a wheel of emotions here if this helps

I'm noticing a less than positive theme here. Let's dig in...
---

Much time is spent at the water cooler maligning the "them" who have forced "us" to create technical debt in the name of _blank_.

We did a poll here, and we know that many have talked about technical debt (and all its forms including testing automation, builds, ci, cd, documentation, and ux).

Everyone agrees it exists, and we all know whose fault it is,

---
not mine. Whose then?

---

the teIm (with the ellusive "I" in team)?

---

If I wanted to perform "intro bait" I'd tell you that it's your fault (too), but I'm not just going to blame the victims here. The whole team has a part to play in this. But as I always tell my kids, "you worry about you" and in this case, you can only change what you do about it!

---

Instead, this discussion will be more like a magic trick. I'm going to make some of it disappear, and other parts are going to magically transport to another dimension. Most importantly, we're going to learn how to do something about it together.

---

I like to say, "everything's a tradeoff". And in generally, we're going to discuss why software is the best profession around.

My friend Genevieve, she's building a new home. Let's pretend she's our customer and walk through the process of building for her. First, we're going to draw her some plans, you might be helping with construction, or you might be helping to inspect the results. Or following all the parallel paths here, you might build things, systems, rules, automation, or anything to make this ecosystem function.

Now let's imagine we were discussing a change to a house we're building. I want you to build out this kitchen to see how it works, put all the counter and fixtures in, paint it, but don't hook up all the plumbing an electricty because I just want to see how it works first so I can make changes if it's not right.

---

You'd throw your cool clipboard at me and run away, or maybe you'd patiently explain how this is a bad plan because we'd have to redo all the floors, walls, fixtures, just to put the plumbing in later even if you didn't make any changes. And if you did make changes, they'd still be super expensive because we might have to bump walls, expand foundations, roofs, etc.

But it depends on your business, if you do rennovations, you start to see $$$ from someone who wants to make changes and think through the permutations.

In software, if we went to modify this kitchen and found our roof wasn't big enough, or there wasn't enough eletricity in the walls, we'd call this technical debt.

---

This problem arises from the beauty that building software allows compromises in so many ways. These compromises show up in ways that would be unacceptable in most products. For example, no one would allow you to build a kitchen on a client site without actually installing plumbing. These types of activities in most other disciplines are done in the "design" phases of a more traditional waterfall-style project, or done with much lower-cost solutions like blueprints, CAD, or small-scale models. What do we do with these artifacts once we've built the house? Keepsakes? trash?

This is a huge benefit! In software we can say things like: let's build this kitchen, but we won't worry about whether we need pipes in the floor until later. We won't worry about whether we'll have two sinks or one sink right now.

---

These tradeoffs are allowed in software because the escalation of costs dwarfs in comparison to most other fields (yes, I know some things are costlier than others). If you decided late in the project you wanted 3 lanes instead of two when building a road, you'd need to go back and regrade the road, buy land, make a new traffic plan, secure additional funding, etc.

This is why agile and software go together so well! As you focus on an agile methodlogy, you can move risk up to the front. Focus on the areas where you need clients to give you feedback so you might decode their cryptic requirements.

---

What's the goal of agile/lean? "Reduce waste"

What does debt mean?

Someone owes someone else something?
"something, typically money, that is owed or due. " - (from <https://www.lexico.com/en/definition/debt>)

---

This is all just WORK and we need to figure out how to manage it.

---

you are thinking, "but my situation is different,"

---


Let's say we run a todo list app.

Someone decides users want to be able to sent a tweet when the finish a task. (twitter icon here)

1. As a user, I can connect to my twitter account so that I can later post my completed tasks
2. As a user, I can click the tweet button after completing a todo item to shart with my tweeps

let's consider alternative futures:
1. We love this feature, and want to roll out tweeting to other places in our app.
graph of rework required over time

2. We decide to use facebook instead, no one tweets any more.
graph of rework required over time

4. We decide to use facebook in addition
graph of rework required over time

5. We decide to use twitter for logins
graph of rework required over time

6. We kill the future

This doesn't look like debt to me. This is some sort of credit default swap



---
# Appendix

let's consider a different scenario

8. add feature for users to set priority with 5 different values
9. change to only 3 values # the point here isn't that there's now TONS of debt, but that debt was created with one decision

our previous concept of technical debt can be "Created" with any decision of product direction.

We've turned this benefit of software into a disadvantage. This type of change and evolution should be encouraged and leveraged. For example, this allows us to build a proof of concept that's not fully scalable and test it on some users. It allows us to test a feature to see if people will use it before we incorporate it into everything we do.

This commonly happens with testing as well. The cycle:
1. product wants feature qucikly, dev writes feature, "not enough time" to write automation, test thourhgly so it gets pushed out the door.
2. Things go great and now product wants feature 2 added on top.
3. Product complains about how long feature 2 is taking, dev complains about the tech debt, test complains about the lack of automation

Everyone here got caught by "techincal debt", but this is a terrible term. better terms here would be software "perspective" or "hindsight"

What really happened:
1. product didn't know if feature was going to get used, or fit the need, so they really wanted to test it with users
2. product was so excited that we rolled it out quickly they forgot that it was just for testing with users
3. dev feels like they got burned for doing what product asked because they built something they're not proud of, cut corners, and left sharp edges
4. test has to manually test each change, because they compromised to help get it out the door and they feel like this always happens where they don't get enough time to write tests

when product asks you to build and estimate, think about all these items, encourage them to participate in the decision making process.

Learn ways to commnicate these tradeoffs, like number of users something will support -- the difficulty of future expansions, etc. Give choices, with both being acceptable.

As we know, our role is to serve the business and offer up the responsible choices. Don't let them talk you out of things that should be done. Honor the testing period.

---------
TODO: think about using polling to compare estimates of tech debt


maybe I could start off with this scenario and back into how do you prioritize automation to dig out of the hole? How do you break the cycle of agreeing to do manual testing in lieu of automation to be a "team player" and "get it out the door".

What can we learn about building technology from Kent Beck's 3x strategy. Explore, extract, and expand - what phases should drive what level of investment?

How do we learn from different investment strategies.

Sources:
1. https://3rd30.com/2019/07/02/episode-042/
2. https://wealthhow.com/types-of-short-term-investments

Shu ha ri?
dreyfus model?
going from basic skills where you should make sure work gets delivered according to spec without sacrificing quality or relying on product to "let you" go back and fix things. Advanced skills where you make compromises based upon the infinite flexibility of software.
