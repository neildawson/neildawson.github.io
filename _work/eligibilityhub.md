---
title: "Eligibility Hub"
description: "Simultaneously building a product squad and a personalised credit commentary feature"
---

In 2021 I moved to a new squad at TotallyMoney, named Mission Improve. We were tasked with “helping customers improve their financial situation and build financial momentum”.

I worked very closely with the product manager, mid-weight product designer, and developers to set the tone for our new team, interpret our remit from the company, and take our first steps towards the company’s long term vision.

We made a long-overdue feature that I’m really proud of. The Eligibility Hub highlights issues with your credit that are holding you back. Crucially, it doesn’t stop there, suggesting actions you can take to make a difference.

Perhaps more importantly for me, we also designed our new team to represent our values and work the way we wanted.

## A new mission

### The business context: building momentum

The business was on a big engagement drive, aiming to <mark>get more customers set up to access their credit report and regularly using our native app</mark>. With other teams dedicated to onboarding and retention, it was our job to build out some strong core functionality the other squads could leverage to accomplish their goals.

Our CPO had recently set a future vision which foresaw a service that intelligently responds to a customer’s financial position. From this vision came the theme of our first major piece of work: “action plans”.

### The product context: lots of numbers, not much guidance

When customers came to us for their credit report we could show lots of data on their credit use, but not a lot of commentary or guidance to make it useful. Much of the really valuable knowledge was buried in FAQs, guides, or deep in the page hierarchy, and very little was personalised.

I came from a squad solely focused on the credit report area of the service, so I was acutely aware of this gap. We knew from speaking to customers that <mark>people mostly came to us for their credit score, but it was unclear why the score matters, or how to improve it</mark> .

My new teammates Tom and Lorraine (product manager and mid-weight designer, respectively) had been working on a similar problem. TotallyMoney had another score, Borrowing Power, an indication of how many credit offers you’re eligible for. Lorraine had conducted research which indicated customers were unsure how to improve this score, too.

There was a lot of overlap in the factors influencing both scores, so it was likely we could kill two birds with one stone. <mark>We were in a great position to address the lack of an onward journey</mark> in both areas.

### Collectively defining our team’s purpose

As a brand new squad with a fairly broad remit from the business, we needed to have a clear idea of what we stood for and what we were trying to achieve.

Armed with a great framework from my colleague Dave, I facilitated workshops to collaboratively define our mission, our vision for the future, and principles to work by. Lorraine and I refined these into clear statements. For example, our mission:

> Everyone’s trying to get somewhere. We show people how far they’ve come, what to do next, and accompany them onward.


<mark>By framing everything as a next step on a journey already underway, we hoped to diminish any sense of intimidation</mark>, motivating people to take action.

## Our first project

### Building a model to narrow our focus

Lots of factors influence your credit score and your eligibility for a credit product. Some of the most impactful are your total credit limit, how much of your limit you use, and missing or defaulting on repayments.

Consequently, there are many actions you can take to improve your scores, so we needed to narrow our focus. <mark>Tom and I built a model of all the factors influencing both scores</mark>. We gathered data points and other considerations, including:

- Impact, or how much weight each factor carried in each score calculation (sourced from supplier documentation and a study by our data science team)
- Number of TotallyMoney customers currently affected
- Quality of the existing experience in our product (if any!)

Now we could see which factors were common to both scores and assess their importance, <mark>we prioritised the list to determine where to start</mark>. We settled on a short list of impactful factors we’d explain to customers in an initial release, planning to follow up with more factors later.

### Proposing a new framework for our product: Atomic Actions

The product squads had been split between two tribes for the past few years, one focusing on product comparison and monetisation, one on the free credit report. This split was evident in the product, with not much connecting the two areas. With the retirement of those tribes, we wanted to eliminate those gaps in the product, too.

<mark>I advocated for the creation of an extendable, modular system</mark> for discussing these factors, rather than building unique solutions for each. This would allow us to optimise effort by building on past work, and hopefully prevent older work from falling behind as shared templates were updated.

It wasn’t just about templates and components, though. Many factors (some of which I mentioned in the previous section) are foundational financial concepts, referenced often. <mark>The concepts themselves should be able to slot in to lots of journeys</mark>, anywhere in the product. For example, talking to someone about missed payments is relevant for people trying to improve their score, overcome debt, prepare for buying a home, and so on.

I called this proposal “Atomic Actions”, pinching the “atomic” concept from [Brad Frost’s Atomic Design](https://bradfrost.com/blog/post/atomic-web-design/). Mission Improve were on board immediately, and I received enthusiastic feedback when I presented it to the whole company. <mark>This became a key guiding force in the project</mark>.

### Sharing work between two designers and a PM

Tom, Lorraine, and I operated as a triad, making key decisions together, then distributing work amongst ourselves to play to our strengths and keep up momentum.

Lorraine was responsible for most of the journey planning, concepting, testing, and design for the hub and most of our first actions. I supported and guided her where needed, which I found really rewarding.

Tom and I worked to create rules of thumb for what determines optimal and suboptimal behaviour for each factor. Lorraine and I then worked closely with the copy team to express these concepts clearly and sympathetically.

I handled one of the factors, missed payments, from end to end. I conducted desk research, analogous research, held an ideation workshop, concepted, then proposed a few possible solutions. I enjoyed working closely with Craig, one of our front-end devs, who carried out a few quick “spikes” to assess the technical feasibility of each solution. <mark>We settled on a simple reminder system we could build quickly to validate the concept</mark>, piggybacking on iOS and Android calendar functionality to get some features for free.

## Results and reflection

![The eligibility hub in motion, showing personalised breakdown of factors holding you back from getting the best offers]({{ "/assets/eligibilityhub/dynamic-actions.gif" | absolute_url }})

The eligibility hub, including the reminder system to combat missed payments, was still in development when I departed TotallyMoney. The hub has now launched and I’m keen to hear how it performed against our engagement goals. I’ll update this case study when I do!

Defining our ways of working together with the squad was one of my most rewarding experiences at TotallyMoney. I’m particularly pleased with the triad Tom, Lorraine, and I established. It’s an effective, reassuring structure that I’d like to replicate in future, ideally with a dev in the mix too.

Looking back, there was a key point where we took stock of all the workstreams for this project and divided them amongst ourselves and a few other contributors. Before, Lorraine had been managing this mostly on her own. On reflection I see that this is just the kind of stuff I struggled with as a junior and mid-weight, so in future I’d do this much sooner, if not from the outset, to bring clarity and confidence, and improve pace.