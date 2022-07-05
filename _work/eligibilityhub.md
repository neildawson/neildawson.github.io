---
title: "Credit Health Check"
date: 2022-01-01
description: "Spurring 20% of monthly active users to take action on their credit, while shaping the purpose of a new product squad"
introduction: >
 In 2021 I moved to a new squad at TotallyMoney, named Mission Improve. We were tasked with “helping customers improve their financial situation and build financial momentum”.
 
 
 I worked very closely with the product manager, mid-weight product designer, and developers to set the tone for our new team, interpret our remit from the company, and take our first steps towards the company’s long term vision.
 
 
 Our first initiative, the credit health check, highlights issues with your credit that are holding you back. The crucial difference to the competition is it suggests actions you can take to make a difference.
 
 
 Perhaps more importantly for me, we also designed our new team to represent our values and work the way we wanted.
responsibilities:
  - "Identifying opportunities and setting direction"
  - "Overseeing a midweight designer"
  - "Desk, competitor, and analogous research"
  - "Facilitating an ideation workshop"
  - "Exploring feasibility with devs"
  - "UX, UI, and concept testing"
results:
  - "Over 60% of monthly active users (MAU) viewed a factor impacting their credit"
  - "Over 20% of MAU took a suggested action to improve"
  - "Now a primary growth driver for the product"
---

## Challenges

### Building engagement

The business focus was engagement, aiming to <mark>get more customers using their credit report and the native app</mark>. With other teams dedicated to onboarding and retention, we were to build core functionality to help people understand and act on their credit.

Our CPO had recently set a future vision which foresaw a service that intelligently responds to a customer’s financial position. From this vision came the theme of our first major piece of work: “action plans”.

### Turning a report into a guide

I came from the squad responsible for our free credit report and had seen a theme across many studies: <mark>customers came to us for their credit score, but didn't know why it mattered, or how to improve it</mark>. We let them browse their data, but didn't offer a lot of guidance.

The product manager (PM) and midweight designer (PD) had been talking to customers about TotallyMoney's other score, *Borrowing Power*, an indication of how many credit products you’re eligible for. They learned customers were unsure how to improve this score, too.

Many of the factors influencing the scores were shared, so <mark>we were in a great position to address the lack of an onward journey</mark> in both areas.

### Defining our new team’s purpose

As a brand new squad with a broad remit from the business, we needed a shared purpose. <mark>I facilitated workshops</mark> to collaboratively define our mission, our vision for the future, and principles to work by. The PD and I refined these into clear statements. For example, our mission:

> Everyone’s trying to get somewhere. We show people how far they’ve come, what to do next, and accompany them onward.

<mark>By framing everything as a next step on a journey already underway, we hoped to diminish any sense of intimidation</mark>, motivating people to take action.

## Setting direction

### Identifying opportunities and deciding where to start

Lots of factors influence your credit score and your eligibility for a credit product, like how much of your credit limit you use, and making (or missing) repayments. Consequently, there are many actions you can take to improve your scores, so we needed to narrow our focus.

<mark>The PM and I built a model of all the factors influencing both scores</mark>. We gathered data points and other considerations, including:

- **Impact**, or how much weight each factor carried in each score calculation (sourced from supplier documentation and a study by our data science team)
- **Quantity** of TotallyMoney customers currently affected
- **Quality** of the existing experience in our product (if any!)

Now we could see which factors were common to both scores and assess their importance, <mark>we prioritised the list to determine where to start</mark>. We settled on a short list of impactful factors we’d explain to customers in the initial release, and defined rules of thumb for optimal and suboptimal behaviour in each.

### Proposing a new framework for our product: Atomic Actions

Many factors (some of which I mentioned in the previous section) are foundational financial concepts, relevant to lots of journeys. For example, addressing missed payments is also helpful for people paying down debt, managing their spending, getting a mortgage, and so on.

<mark>I advocated for the creation of a modular system</mark> for factors. This would allow us to reuse our work in other areas in the future, and keep a consistent experience between factors.

{% include figure.html file="/assets/eligibilityhub/atomic-actions.png" caption="Excerpts from my presentation to the company about the project and my Atomic Actions proposal. I used the Lego blocks metaphor to show how we could save time and improve consistency across different journeys." %}

I called this proposal “Atomic Actions”, pinching the “atomic” concept from [Brad Frost’s Atomic Design](https://bradfrost.com/blog/post/atomic-web-design/). <mark>This became a guiding principle for the project</mark>, and it was received enthusiastically when I presented it in a company-wide meeting.

## Design

### The hub

![The credit health check in motion, showing personalised breakdown of factors holding you back from getting the best offers]({{ "/assets/eligibilityhub/dynamic-actions.gif" }})

I supported and guided the PD, which I found really rewarding. She was mostly responsible for the hub itself, and we collaborated to establish a template that worked for all factors, choose entry points, plot out the journey, prioritise and label factors, and write clear and sympathetic descriptions.

### Missed payments

In addition to the strategic work described above, <mark>I handled the missed payments factor from end to end</mark>:
- Desk, competitor, and analogous research
- Investigating principles for behaviour change
- User journey map
- Facilitating an ideation workshop
- Ideating and prototyping solutions in Figma
- Concept and usability testing
- Feasibility investigations with a front-end dev
- Constructing the UI with our component library

{% include figure.html file="/assets/eligibilityhub/experience-map.png" caption="I made this experience map, based on research findings, to help ideation workshop attendees understand the problem area and see things from another perspective." alt="The experience map shows the journey of a customer who misses a payment, at each step noting their thoughts, pain points, and opportunities." full-width="true" %}



### The first missed payments action

I explored lots of possibilities for the first action, like searching for direct debit instructions, searching for your lender's contact details, and setting up a reminder. <mark>We were looking for something simple, lovable, and complete</mark> that we could build quickly to validate the concept.

Setting up a reminder was the most promising opportunity, and there were lots of ways to do this, too. We considered using our newly minted push notification system, email reminders, and integrating with the calendar or reminders apps on your phone.

I worked closely with one of our front-end devs, who carried out a few quick “spikes” to assess the technical feasibility of each option. <mark>He and I decided to provide reminders through integration with the iOS and Android calendar</mark>, piggybacking existing functionality to get some features for free, like editing and push notifications.

<figure>
<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/zswYOL1WA70?controls=0' frameborder='0' allowfullscreen></iframe></div>
<figcaption><p>I designed the screens for the missed payment factor in Figma, and made this prototype to demonstrate the process of setting up a reminder. At the end I show what happens when the customer denies the request to access their calendar.</p></figcaption>
</figure>

Every factor also included two generic actions: disputing incorrect information on your report, and adding a correction to your report.

## Results

The credit health check launched in January 2022. In its first 6 months over 60% of monthly active users (MAU) viewed a factor impacting their credit, and <mark>over 20% of MAU took a suggested action</mark>. The missed payments factor was the most interacted with. As a bonus, rates of customers reporting errors in their credit report rose noticeably.

Mission Improve dangled this carrot in front of customers through emails, push notifications, and additional entry points. <mark>It has become a primary growth driver for the product</mark>.

Defining our ways of working together with the squad was one of my most rewarding experiences at TotallyMoney. I’m particularly pleased with the triad the PM, PD, and I established. It’s an effective, reassuring structure that I’d like to replicate in future, ideally with a dev in the mix too.