---
layout: post
title: "The News Tree: Software Product Proposal"
date: 2011-08-01 12:00:00 +0100
categories: 
---
		
<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://player.vimeo.com/video/27462583' frameborder='0' webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe></div>

## Design

### Interface

All News Trees begin life as a blank canvas:

![An empty news tree]({{ "/assets/knightmozilla/blank.png" | absolute_url }})

To grow a news tree, the user must provide an ‘acorn’ (a document, link or other piece of media which can be mined for information) or use the built-in tools to find one. With HTML5 we can accept pasted links or files dragged from the desktop, making it easy to get started.

The user can add sources of their own or search for new acorns:

![Adding and finding sources]({{ "/assets/knightmozilla/Add1.png" | absolute_url }})

Narrowing the search to a particular region and period of time allows us to pinpoint primary sources – invaluable to a well-rounded story. If the user does not provide these details the system will try to retrieve it from the supplied source.

Trees are born from acorns:

![An acorn]({{ "/assets/knightmozilla/Add2.png" | absolute_url }})

The user can build a tree entirely from their own sources (for example, to demonstrate the core elements of a story, or highlight a particular viewpoint) or use the branch tool to find a myriad of sources before pruning their tree down to size.

'Add source', 'prune' and 'branch' (the verb!):

![Adding, pruning, and branching]({{ "/assets/knightmozilla/Buttons.png" | absolute_url }})

There are three simple controls available to the user: + opens the add source dialog, – enables pruning mode where branches or comments can be removed, and the branch tool forces growth in a branch or acorn, drawing more sources around it.

This acorn has branched three relevant sources:

![New branches]({{ "/assets/knightmozilla/Add4.png" | absolute_url }})

### Behind the Scenes

Sources are gathered in a number of ways.

First of all, data is parsed from existing sources or the user’s search query. This information is used to seek sources directly from a central list of outlets (very diverse, but not exhaustive: BBC, Twitter, WhiteHouse.gov, [think tanks](http://www.fpri.org/research/thinktanks/GlobalGoToThinkTanks2010.pdf) etc) via their own search tools or APIs. With an established net of sources, digital trails like blog trackbacks, direct replies, comments and mentions on other sites are followed to trace a second batch of sources. This technique can be repeated to gather a very wide range of sources.

Sources are rated by relevance (measured by matching keywords, shared branches etc) and reliability (with metrics like Technorati rankings). Typically only recognised sources which most closely match those on the tree will be added, but social media commentary and occasional ‘wildcards’ are included in pursuit of balance.

Metrics and metadata directly influence the appearance of objects in the visualisation:

![Key]({{ "/assets/knightmozilla/Key.png" | absolute_url }})

Developers and designers would work closely with researchers and journalists to gather [heuristics](http://en.wikipedia.org/wiki/Heuristic) and build a library of reliable first sources in order to refine the search algorithm.

Through custom CSS stylesheets, trees can be adapted for branding purposes, personal preference or disability. Trees can be embedded anywhere that allows direct HTML manipulation, and hosted at a central domain.

## Business Brief

The News Tree brings benefits to all corners of the newsroom – saving time, effort and frustration – and augments rather than replaces existing infrastructure.

### Interaction Designers

Shazna Nessa told us that staff in interaction departments of large news outlets must always be prepared to drop their scheduled work and prioritise visualisations for breaking news items. Though by no means a replacement for a bespoke solution, by feeding in select sources a small news tree can be quickly constructed and embedded. This bonsai news tree serves to communicate [the foundation of the story](http://www.bbc.co.uk/news/uk-14124020) in lieu of the final visualisation.

### Researchers and Analysts

Larger newsrooms have dedicated, internal staff whose role is to conduct research and prepare briefs for journalists. Not only does a News Tree simplify and speed up the task of seeking out sources (particularly via social media), those trees can be pruned (or a new tree started) to create an interactive primer on a story – more engaging than any text brief.

### Journalists and Reporters

In the field or in the newsroom, mobile or desktop, staff can create and manage collaborative resource libraries, save sources for later perusal and build story ‘sketches’ before putting pen to paper.

### I.T. Staff

Newsrooms by their nature don’t require the highest spec computers, their primary uses being word processing and internet browsing. By building the News Tree open-source and in-browser, based on standards like HTML5, we ensure that even the most decrepit machines in the smallest newsrooms will be able to run the tool, with no dedicated software to install or maintain. By maintaining a user-centred approach to design, we also ease the transition of the technologically unenlightened into the world of social media.

Perhaps most crucially, the News Tree is a free, customisable, open-source tool, meaning its users are able and encouraged to find new applications not foreseen by its creators.

## Competitors

Automated news aggregation tools like Google News, Tattler and Meltwater perform a similar role in collecting and filtering scattered sources. However, not all of these solutions are free or open-source, and none have the same level of visualisation found on a News Tree. By moving away from text-based browsing we take advantage of the visually orientated human mind, presenting a broad overview which enables swathes of sources to be rapidly scanned by eye.

Crowd-sourced tools like Reddit are extremely powerful, if fickle. For this reason the News Tree is not solely automated. The user can grow their tree automatically, or build it exclusively from their own sources.

## Open Issues

The News Tree was conceived as a way to bypass curation through automation, but it has turned out as a tool in which automation is used sparingly, if at all. As with all tools, it is up to the user to wield it responsibly.

It’s very easy to write about the effectiveness of a hypothetical algorithm. Of course, creating the back-end for the News Tree will require a great deal of user research and close collaboration with developers.

The simplified style of tree used here reflects the need to develop the rating system further.

Burt Herman warned us of letting our projects become Swiss Army knives, but we were also told to “think big and bold”. I think I’ve struck a good balance.

## Thanks

For their invaluable feedback:
- Michael Aitken, Sports Writer
- Louisa Brooke, Foreign Affairs Analyst, BBC
- Jonathan Duffy, Planning and Production Editor, BBC
- Rhona Grieve, Special Events, BBC
- Jamie MacDonald, News Reporter, Evening Express
- Matthew Rhodes, Special Events, BBC

For helping me develop the idea:
- [Ross Forrest](http://twitter.com/#!/rssfrrst)
- [Linsey MacIntosh](http://twitter.com/#!/linseymcintosh)
- [Chris McNicholl](http://twitter.com/#!/cmcnicholl)
- [Shaun McWhinnie](http://twitter.com/#!/himseelf)
- [Lynsey Smith](http://twitter.com/#!/lynsey_smith)
- [Michail Vanis](http://twitter.com/#!/mikevanis)

Map image credit: [madmaxpayne](http://madmaxpayne.deviantart.com/art/World-Map-with-Borders-PSD-96083532)