---
title: "Ideas for a fair review system in Software Engineering and beyond"
categories:
  - blog
tags:
  - Research
  - Science of Science
  - Reviewing
---

By my very crude estimate, there are at least 15,000 reviews done
every year in the top-20 Software Engineering conferences and journal
alone to assess the quality of submitted manuscripts. Assuming that a
review takes on average at least 2.5 hours on average (in reality,
much longer!), this amount of work equates to a mammoth 27 full-time
jobs.

![Reviewing overload](/assets/posts/reviewing.jpg)

What is puzzling is that this Herculean task of reviewing in its
current form hinges entirely on volunteers providing free reviews In
Software Engineering, we have seen many recent help calls that say the
current review system
[no](https://2016.icse.cs.txstate.edu/static/downloads/2016ReviewProcess.pdf)
[longer](http://www.icse-conferences.org/sc/ICSE/2017/ICSE2017-ChairsReport-TechnicalTrack-v1.0.pdf)
scales, with
[some](https://twitter.com/AndreasZeller/status/1500082985013596163)
individuals providing more than 100 reviews annually. This problem is
exaggerated by a system that has no memory of prior reviews across
venues and by authors who re-submit articles with little to no changes
to different venues, triggering a new set of reviews, essentially
treating reviews as a free resource. Moreover, typically, the same set
of people are found in Program Committees again and again. We also
know that well-knonwn members of certain, already under-represented
groups (such as women in Software Engineering) often take on a
higher-than-average reviewing load, being invited over and over
(perhaps to fill the gender gap?), while it can be be hard for others
from the same minority group to be invited at all. This leaves the
question of how one ensures that everyone in the community can and
does contribute, if not equally, then in proportion to the number of
articles they submitted. Some academics have hard-and-fast rules they
commit to, but the [range of how many reviews to perform among just
three persons is
huge,](https://twitter.com/AndreasZeller/status/1500082985013596163)
with a 4x difference. Clearly, we need a system to not be reliant on
gut feeling or on individuals' diverging gut feel for what constitutes
a fair amount.

# Why a simple system is bound to fail

It is immediately obvious that a simple system to ensure review load
fairness does not work because papers are submitted by a (variable)
number of authors, instead of just one. Moreover, the most simple idea
to ensure fair reviews would otherwise be "You can submit here if you
have reviewed here before" does also not work because (leaving aside
the chicken-egg problem for a moment) because of a limited review pool
for each venue and not all reviewers being able or qualified to review
for a given venue.

# A credit-based review system

I have long touted the idea of a *credit-based review system,* but
never written about it publicly. In this post, I want to lay out the
possible logistics of it. Similar to Machine Learning-based solutions,
there might be some hyper parameter tuning and optimization in order,
depending on how it plays out in practice. Regardless, the idea hinges
on a substantial number of venues in a field taking part, which is an
admittedly difficult to overcome initial hurdle. The system could be
orthogonal to EasyChair or HotCrp, and connected to them, identifying
submitting authors by their ORCID. Identification, a problem many
sites face, should not be a hurdle, either, because authors have a
very strong inherent motivation to submit under their (and only their)
real name.

## Submitting

Being allowed to submit to a venue requires a certain number of review
credits being present. This could either be the sum among the
authorship or taken from each author individually. Upon submission, X
credits are deducted.

For beginning PhD students, or just to get the system started, every
person signing up should be awarded a number of fixed credits (similar
to when the Deutsch Mark was introduced in 1948, where [every citizen
received 40 Deutsch
Marks](https://en.wikipedia.org/wiki/Deutsche_Mark#History)). If we
want to go fancy, we could make this dependent on the current position
of the person: Perhaps an industry researcher is entitled to 2
credits, while a PhD student might receive 5.

## Reviewing

Similarly, after delivering a review, a reviewer gets Y credits
awarded. *This system could tackle the problem of declining review
quality, too:* guarantee a minimum rate for a review, and depending on
the quality, more credits could be given.

A similar thing could happen for more prestigious venues (actually,
this would be perhaps the first objective marker for them to tout
themselves as such) or journal manuscripts, where more credits could
be granted.

## Toward an economy of reviewing

Many academics currently decline invitations to PCs or, more severely,
I think, journal paper reviews: I have come across a TSE article that
had an unbelievable 40 academics rejecting to review; needles to say,
I declined, too (I did find the person to finally review, it, though;
thanks, [Annibale](https://apanichella.github.io/)!), for there is no
tangible benefit of reviewing for them. As soon as you can not submit
a paper because you do not have the required credits, this changes!
The famous [number 3 ICSE rule from
2017](https://icse2017.gatech.edu/?q=technical-research-cfp) could
perhaps be avoided by this system, too: authors simply would not have
been able to amass the required review credits.

When deciding on a pool of reviewers, I as a chair was recently faced
with a candidate pool twice the required size of absolutely equally
qualified candidates. [In the end, decided to select among them by
chance.](https://inventitech.com/blog/chairing-the-fse-industry-track/)
A system could instead have looked at the number of reviews they each
already performed in the past year.

A market-based system, I like the possible inherent fairness this
would involve. Think about it to the extreme, there could even be a
monetary price for a review credit (if, similar, to the European
emission system, you want to allow transfer of credits): this could
enable authors from industry who would not have an opportunity to
review, to submit, too by buying credits.

# Is reviewing really without benefits?

In this discussion, I have not really mentioned publishers much. This
is because I think in a future academic system, there is simply no
room for them. Alas they also would be the best place to kick-start
this system, with the exception of IEEE/ACM, which would be even
better (think about Elsevier requiring you to have credits for
publishing there). Of course, you currently get the very questionable
offer of a 50% discount on "the publisher's" latest overpriced
offerings.

Currently, much of the debate focuses on reviewing as solely an
altruistic contribution to a functioning ecosystem. While I think that
this is largely a valid stance, it falls somewhat short of reality:
Receiving direct pay for reviewing is seldom, but does happen, like,
for example, the comfortable rate reviewers for the European Union
receive, for example for ERC grants (granted, I have applied and many
people I know, too, however, no one ever heard back from them
... strange). Apart from direct monetary benefits, reviewing (and, if
you will, as an extension of reviewing) chairing gives one extra
ordinary visibility within the community. This 'academic' fame can
come in handy at numerous occasions, for example, establishing oneself
as a senior academic or when externally certifying expert status, for
example, for visa purposes.

# Conclusion

In the end, the implementation of this system technically should be
pretty straight-forward, and in my opinion, has benefits over simply
spreading the gigantic review load of 27 full time positions in
Software Engineering alone, fairly across a large number of people: It
might help visibility of underrepresented groups, it would free up a
large amount of time of the currently pretty elite reviewers, and it
certainly would eliminate the free riders of the current system. Of
course, many current reviewers would argue that they do this for free,
because they like it, or because they are uniquely qualified. But in
light of a systemic problem, I would love to have that discussion.

Of course, one could say that exceptional service is one way to get
yourself known and contribute to the field. If we systemize that, this
might go away. I guess this depends on the final market economics of
reviewing, which I do not claim to forsee now. We can always tweak the
system such that **one does not get away with not doing any community
work**, while no else suffers. Another argument is that not every
person is equally qualified to review, and I agree, too. However,
assigning different number of credits per review and [moving towards
reviewing standards](https://arxiv.org/abs/2010.03525) should
alleviate these concerns.