---
title: "Live Alerts"
description: "Bending a commercial tool into meaningful customer notifications that outperformed our best campaigns"
introduction: >
 The credit reporting system is designed for lenders, not consumers. These days we can all access our reports, but it’s usually still difficult to make sense of all the data. 
 
 
 When TotallyMoney gained access to a new daily feed of significant credit report changes, we set out to bend this tool for lenders into a customer-centric service, while boosting app engagement.
 
 
 Timely messages to customers about meaningful changes in their credit profile easily outperformed our typical reactive emails, and made a great test bed for our first push notifications.
responsibilities:
  - "Analysed and documented the API"
  - "Jointly selected our first alert"
  - "Revamped UI and IA for native and web"
  - "Drafted and A/B tested copy for email and push"
results:
  - "37.04% click-to-open rate on our first alert"
  - "40.67% click-to-open rate on the second"
---

## Assessing our options

When we got our hands on a new API that highlighted changes to our customers’ credit profiles, we started digging through the list of over 200 status alerts. It was time for some spreadsheet magic.

First, my Product Manager and I worked with the data provider to clean up the list, stripping out duplicates and system alerts that weren’t useful to customers. Next we <mark>assessed the remaining items by lots of factors of our own devising</mark> like contribution to our OKRs, impact on the credit score, and how well we explained the subject in our product.

Knowing other teams at TotallyMoney would be keen to use this service in future, <mark>I condensed all my knowledge into a human-readable summary</mark> of the major topics and the associated data points, so they could benefit from our knowledge and not start from scratch.

## Choosing our first alert

Steadily whittling down the 200 items to shorter and shorter lists, we settled on “hard searches” for our first release.

### What’s a hard search?

Every time an organisation looks at your credit report, they leave a footprint in the form of a search record. They come in “hard” and “soft” varieties, and the former are more meaningful for a couple of reasons.

Hard searches usually only happen when you apply for credit, and lenders are hesitant to lend if you make too many applications in a short time.

### Why this alert?

Every new hard search recorded on a customer's credit report was an opportunity to:

- **Show customers how their actions were represented in their report**\
We knew much of the credit report was mystifying to our customers. Here we could demonstrate cause and effect.
- **Prevent rejections caused by too many applications**\
We knew it was not common knowledge that multiple hard searches can count against you. 
- **Say something timely**\
Most of the other alerts were weeks or months old, due to lender reporting delays. In this case you’d be notified the same day your report changed.
- **Spot identity fraud immediately**\
We didn’t expect it to happen often, but we’d still be showing customers we were looking out for them.

We were confident there was real customer value to be had.

### Why not?

- **Low volume, about 100 instances a day**\
We thought this would be fine for our first release. Later I’ll explain why I might choose differently in retrospect.
- **Our in-app experience for browsing search records was poor**\
The information architecture was unclear, and the layout was broken by a recent redesign.

I pushed to include a redesign of the searches area as part of this project, so we’d have a satisfying end-to-end journey.

## Design

Besides tidying up the broken UI and improving the IA, I was also keen to improve our explanation of the distinction between the two types of searches. 

I won’t dwell too much on how I got there, as these things are covered in my other case studies, so in summary I: mapped potential journeys, facilitated a sketching workshop, collaborated with our UI specialist on required components not found in our design system, carried out ad-hoc testing of the new IA with some colleagues, and drafted copy for email and push notifications – amongst other things!

## Results and reflection

### Excellent open rates

The hard search alert email clocked in with a 32.55% open rate and a <mark>37.04% click-to-open rate</mark> (CTO). Our best performing emails until then topped out at about 23% CTO, so this was clear validation of the personalised alert initiative.

Our next alert informed customers of new accounts appearing on their credit report, a piece of work I started before handing over to another team during a reshuffle. It performed even better: 40.67% CTO.

### A call to action outperformed an explanation

![A live alert about a new account on your credit report]({{ "/assets/livealerts/live-alerts.gif" | absolute_url }})

We ran an A/B test to learn a bit about how copy in a push notification affects open rates.

Ideally a push notification should be meaningful and valuable on its own. I was keen to avoid clickbait: teasing something important and hiding the full message in the app. 

For compliance reasons we couldn’t name the organisation in our messages, only in the app. Concerned this lack of transparency might worry customers, I proposed an option which explained *why* a hard search is made. We tested this against a version which instead directed customers to open the app for full details.

<mark>Version A (the call to action) performed best, with a 14.64% lead</mark> in clicks per send, and was selected for the full release.

So we learned a bit about how to write engaging push notifications. Obviously, <mark>an A/B test couldn’t tell us if the message worried anyone</mark> unnecessarily, something I’d like to explore further one day!

### A lesson in balancing customer and business value

As I mentioned earlier, hard search volume was not very high. We thought this wouldn’t matter much, as we’d quickly follow up with other alerts, building a library of many low volume messages, instead of a few large volume messages.

Unfortunately, our unique tech stack at TotallyMoney led to a lengthy delay in launching our push notifications system, which contributed to further alerts being put on hold.

Looking back, hard search alerts had loads of value for the customer, but there were just too few of them to meaningfully contribute to our OKRs. <mark>Given the choice again, I’d place more weight on the business goals</mark>  and not rely so much on future roadmap items to deliver the business value.