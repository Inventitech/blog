---
title: "Lessons Learned from Chairing ESEC/FSE 2021 Industry Track"
categories:
  - blog
tags:
  - Research
  - Science of Science
  - Reviewing
---

While ESEC/FSE 2021 is in full swing over in the virtual clowdr world, I thought it'd be a good time to reflect on how it was to chair its Industry Track together with [Miltos.](https://miltos.allamanis.com/)

Before I accepted the offer to chair, I asked myself three questions:
* Am I a good fit (litmus's test: do I know the conference? Have I submitted there before?)?
* Who is my co-chair (super important, as it later turned out!)
* Do I bring something new to the table?


For the last point, I studied the [previous years' CfP.](https://2020.esec-fse.org/track/esecfse-2020-industry-papers?#Call-for-Industry-Papers) I noticed that it was somewhat in-cohesive (looked like several additions were made over many years, but no one really went over it in its entirety), innovations in reviewing were not present, and that it was a bit unclear what Industry track authors and reviewers really wanted. Therefore, we [completely re-wrote the CfP.](https://2021.esec-fse.org/track/fse-2021-industry?#Call-for-Industry-Papers)

# Governing principles

When Miltos and I took over, we quickly agreed on three governing principles:
* Make the track as open and transparent as possible.
* Integrate innovations in reviewing.
* Reduce unnecessary workload on authors and reviewers.

# Author wishes

Most SE conferences' Industry tracks were still single-blind (and certainly of the premier conferences; with the [exception of ICSME](https://www.felienne.com/archives/5467). A frequent counter argument against this was that important industrial context would often be lost, or make the submitted manuscript awkward to read. As a result, we made blinding optional for authors. I am happy to report that not only did 33% of submissions follow up on this choice, but also that there were no complications reviewing these blinded submissions. 

Another important factor for authors is that anecdotally, many feel obliged/are forced to write rebuttals, even for fruitless submissions. To ensure this does not happen, we transparently communicated the paper's score together with the initial set of two reviews; papers with a very negative assessment (at least one strong reject and another reject) would be auto-rejected, unless reviewers saw the need not to do so. For the 17 submission we early-rejected, no reviewer saw the need for this. Instead, it allowed authors to get early feedback, allowed them to re-work their submissions, and us to save the potential burden of a third review. Similarly, we early-accepted 14 papers, again saving the burden of (feeling to) having to write a review for submissions that would anyway make it in.

# Reviewing wishes

In times of corona, it was really hard for us to predict how many submissions we would receive. In addition, unfortunately, we could not get that info for the 2020 edition of the Industry track. As a result, we predicted conservatively to receive 30% more submissions than 2019 (in fact, we received +50%!).

In addition, we wanted to give particularly more junior and Industry people a chance to review, and not limit it to our personal networks. As such, we designed a PC consisting 50% of people we know we could trust and 50% nominations, shared via Twitter (if anyone knows of a better platform to reach academics in SE, please let me know). We were unsure whether we should allow self-nominations (you do want to have reliable reviewers), and fortunately ended up doing so: 100% (!) of nominations were self-nominations, and self-nominated revierwers ended up not being less reliable than our contacts. However, we vetted all nominations. Because everyone seemed like a great fit and we had 50% more nominations than we needed, we simply randomly chose among the nominees.

What helped keep review load down was not only enlarging the PC, but in particular early accepts and rejects. Moreover, we think having 2 reviews for these submissions did not significantly influence review quality.

# What we could improve

![Procrastination graph.](/assets/posts/2021-08-26-procrastination.png)

Even so, there was one main item (and two smaller things) that we would change if given the chance to chair again. Above, you see the review procrastination graph. What was a bit shocking to me was that after our internal deadline, 30% of reviews were missing! Personal reminders helped a lot initially, but then the influx of new reviews dwindled. Similar to stocks, by spreading the review load wide, we effectively hedged against a total default, but would have had to factor in a number of reviews being late. In all this, it was good that we left enough buffer between the internal deadlines and the officially announced ones. Still, the obvious solution for this would be to have an emergency PC of roughly 5-10% the size of the PC.

Moreover, perhaps we shared too much information with authors (making reviews immediately, even before we summarized them with an email), which caused a bit of confusion. Finally, there were a few submissions on which both Miltos and I were conflicted, so we had to override the conflicts.

# What went well

We received a (likely) record number of 61 submissions, and quite accurately predicted this. Out of those, we accepted 23 (39%). With an increased PC and a new reviewing mode, we could still reduce the average review workload to 3.5 in the first round and only 1 paper in the second round. We were also able to acquire new reviewing blood via the (self-)nomination form. FSE was the first major SE conference to use optional double-blind submissions; we are happy to report that not only did a third of the submissions make use of this, but that it also caused no problems during reviewing. When we desinged all this in the beginning, we had no idea that HotCrp technically supported all our non-standard ideas  (e.g., sending out early-rejections). While it definitely lacks a user friendly interface, we were at least able to botch everything. It was also great to work with Miltos, who was pro-active and helped out when I wasn't available. Finally and most important, we were able to keep all deadlines.




If future chairs want our material, we archived everything, which hopefully makes chairing the track in the future much less work. A big thanks to Andrew Bagel from the 2019 edition of the FSE Industry track, who provided us with valuable insights.

