---
title: Three self-intros
author: Colton Grainger
belief: likely
---

After a contemplative and absurdly open-ended summer, I wrote three descriptions of myself and my goals for folks who I might look for mentorship from. Given their positive feedback, I'm posting my initial outbound emails.

The first message was intended for the maths department at CU, the second was a cursory message sent to the programming languages mentoring workshop (Stephanie Weirich had solicited applications on twitter), and the third was sort of a long-overdue thank you card to Issa Rice.

## CU Boulder maths dept

*(1) what are your goals for graduate school*

I aim to make novel contributions to the field of applied algebraic topology.

Upon completion of a PhD, I want to be a researcher for a university, governmental agency, or non-profit organization. I would like to work in a English- or German-speaking metropolitan area that's dense enough to have its own subway/rail system.

For now, I am glowingly glad to be coming to a community of mathematicians and exact scientists at CU Boulder.

*what particular challenges do you foresee for yourself?*

I do look up to academics who published early and often in their research careers (Jean Yang, Matt Might, Scott Aaronson, Philip Guo, among others). I think I've chosen such prolific role models in compensation for my attending a liberal arts college in rural Idaho, from which I graduated in 2016 feeling provincial and green.

I anticipate I will be challenged to pace my ambition---especially what I have imported from wildly successful academics---against the reality that algebraic topology has a very long build-up to research level publication.

## PLMW@ICFP 2018 travel scholarship application

*Please briefly describe any research or technical projects that you have worked on or plan to work on.*

My research interest is in applied algebraic topology, specifically topological data analysis (TDA). I aim to implement a natural type-system for TDA such that (i) a TDA workflow can be composed of strongly typed functional programs, (ii) details of each program's implementation can be hidden when reasoning in an algebraic context, (iii) each program can be type-checked (assuring modularity) and, if possible, mechanically verified.

As a first year PhD student, I have yet to formally take an advisor; however, Prof Agnès Beaudry's research on Computational Chromatic Homotopy Theory (DMS-1612020/1725563) is the clear (and significantly deeper) semantic dual to the syntax I hope to employ when implementing a type system for TDA.

(In terms of my preparedness to understand the workshop: I have a familiarity with Haskell, Scheme, and typed lambda calculus from recent independent study. I have experience with category theory from my undergrad. I have a naive appreciation of homotopy type theory.)

*Why would you like to attend PLMW@ICFP?*

In the first two years of my PhD, I want to structure iterative paper submissions on a tractable project in TDA. While my intended audience includes algebraic topologists, category theorists, and type theorists, I believe that type theorists (and the PL community at large) are the most approachable.

Why?

1. Great PR. As publicity chair for POPL 2018, Jean Yang recorded and posted interviews from a broad cross-section of PL researchers, with the explicit purpose of "conveying to the potential new members of the POPL community ... what POPL is about." 

2. GitHub. The "constellation of artifacts" accompanying PL research is largely showcased in public git repositories, together with commit histories, issue threads, and pull requests.

3. No absurd entry barriers. In his POPL interview, Xavier Leroy mentioned "I was admitted in ENS, Ecole Normale Supérieure in Paris, which is the church of French mathematics. I really wanted to do math. Then, I found out that math was more difficult than I thought. Their courses were really hard and they didn't make them very accessible. They wanted to find the next Fields Medalist." I think the attitude is different in the PL community, where initial contributions need not be world-class. 

So, in summary, I hope to attend PLMW@ICFP because I believe the PL community is approachable, and I want to get a sense of the tools I would use and of the realistic goals I should set for myself to produce a type-system for TDA. 

And lastly, I want to hear Weirich and Polikarpova speak, as they are both role models to me, and I admire their work (in hs-to-coq and Enforcing Information Flow Policies, respectively). 

## Cold email to Issa Rice


I have kept abreast of your [content creation](https://issarice.com/content-creation) since last September, and I wanted to say thanks:

- for holding up a light to demonstrate what an open notebook is and can do
- for references to gwern, Aaron Swartz, and Vipul Naik
- for writing that hauls, tows, and tracks beginners (like myself) through the intermediate steppes of establishing a canonical online identity, finding a voice, finding a project, etc.^[ I notice I tend to especially stiffen up and turn verbose when I'm first talking to people. It can get over the top. Like, I wanted to reference Bulgakov's *The Master and Margarita* to compare some [drama](https://en.wikipedia.org/wiki/Wikipedia:Miscellany_for_deletion/User:Riceissa/Animal_Charity_Evaluators) with [WP:COIN](https://en.wikipedia.org/wiki/Wikipedia:Conflict_of_interest/Noticeboard/Archive_113#Vipul.27s_paid_editing_enterprise) to Pilate's deliberations and decision to turn Yeshua Ha-Nozri to the Sanhedrin. But really. It's a cold first email. I have to draw the line at literary references likening the involved parties to mythomorphic divine figures.]

I studied maths/physics through undergrad (and will return to grad school this fall), but for the last two years I've done service work: a year in medical case management at a refugee resettlement agency in Houston, and a year at a homeless shelter in Olympia. I am motivated by your writing to become a stronger programmer, and to find a niche in which I have comparative advantage to do the most good.

I'd like to setup a database for my friend at the resettlement agency (something like mnemosyne, but instead of flash cards, it displays a short English language health bio for clients who otherwise have limited English proficiency), and I'm wondering if you could point me to (sort of introductory) examples where you've used mySQL[^mysql] or SQLite.[^sqlite]

<hr>

[^mysql]: Issa kindly replied, "For MySQL, maybe going back in the commit history of one of my projects would be easiest, e.g. <https://github.com/riceissa/aiwatch/tree/41956844f204cd01f0e9bf401774ce62bea03104/sql> shows a fairly minimal setup. (The downside is I can't guarantee there aren't any syntax errors for arbitrary commits in the history.)" 

[^sqlite]: "For SQLite I think I've only used it for one project. You can find the schema for that at <https://github.com/riceissa/wikidossier/blob/master/schema.sql> and insertion stuff at <https://github.com/riceissa/wikidossier/blob/f477b6b2f9e0448d20a27bdc54e817d21f64b18d/wikidossier.py#L79-L101> The tutorial I used while making that is <http://flask.pocoo.org/docs/1.0/tutorial/>."


