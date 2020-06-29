---
title: "Why I will never join an Artifacts Evaluation Committee Again"
categories:
  - blog
tags:
  - Research
  - Science of Science
  - Reviewing
---

Recently, I served in the Program Committee of the [Artifact Track of
ESEC/FSE
2020,](https://2020.esec-fse.org/track/esecfse-2020-artifacts) a major
Software Engineering conference. I agreed because I wanted to help a
friend and I think we need to strengthen the academic principle of
being able to check and reproduce findings. Moreover, their idea
sounds simple enough: You install a bit of well-documented software,
you let it run for a bit, and you check whether the results in the
paper matched those produced on your computer. However, in practice,
my experience was less than ideal. In this blog post, I want to talk
about why and make suggestions for future artifact tracks, helpful
hopefully for authors, reviewers, and chairs alike.

![Poor Photoshop of ACM badges](/assets/posts/2020-06-26-acm-badges.png)

## 5 Artifacts to review is ... 4 too many?

Reviewing an artifact means means to develop deep understanding of
often years of work by a group of authors. I find it deeper than
during a paper reviewer. Typically, one has to understand the paper,
the artifact, their connection, and how to run it all. In practice,
for ESEC/FSE 2020, with 5 papers, this was a Herculean task for me. It
also required constant context switching since you have to work on
multiple artifacts simultaneously to meet the tight deadline (10 days
for reviewing).

***Suggestion:*** Assign one or two artifacts per reviewer.

## Interactive sessions cost time (and nerves)

For ESEC/FSE 2020, there was a one week period in which authors and
reviewers should converse and tackle problems on GitHub. This makes
evaluating artifacts much more cumbersome than reviewing a paper,
which is mostly a one-off task you can freely schedule within 2
weeks. There is also no clear guidance on how fast one should come
back to authors in case of a problem. I, for one, have the opinion
that I should not be required to hot-patch code in the artifact with
an editor. I still did because I wanted to help the authors. There is
really no ethical norm on what constitutes good artifact reviewing and
how to ensure all artifacts are treated equal. All my artifacts
required multiple interactions with the authors to either get them to
run or reproduce the results in the paper. 

***Suggestion:*** Limit the number of interactions per artifact (i.e.,
authors are allowed 2 clarifications) or limit number of artifacts to
review (see above).

## Please have your local supercomputer at hand

0 out of the 5 artifacts I reviewed would have run on my
laptop. Unfortunately, the system requirements were not always
documented, so I partly found out after crashing my system or
overheating the CPU. Not sure how to solve this for folks who do not
have access to such hardware? I imagine it is quite embarrassing to
have to come back to the chairs after the artifact assignment and say
"erm, sorry, I can actually not review any of these five papers."
Another question is that many artifacts require one to install arcane
software or apply dubious system changes, which brings me to the next
point:

## Nothing works out of the box ...

... except for the one artifact that used a Vagrant image! Is it a
good use of reviewers' time to having to figure out an install process
(and typically, a myriad of error messages the original authors had no
chance of foreseeing)? I think not. A small minority of programs
(e.g., benchmarks) might not want to use virtualization. All others
(and this should really be 99%): Please, use an image or
container. Note also that having an image does not make it harder to
install the software elsewhere (the conditions on the environment are
in the image, or even better, in a Docker file).

***Suggestion:*** A virtual machine image should be
   mandatory. Considering the zoo of virtualization solutions
   (containers, images, app images), I would even prescribe a certain
   format for a given track. Exemptions from it should be rare and
   require explicit permission.

## This convenient 154,000 line log file reproduces the results.

Oh, of course, one needs to parse it to get the aggregated results in
Table 2, but never mind. Just figuring out what output has been
produced where, and to which piece in the paper it relates is often a
Sisyphean task. Too many artifact documentations, which are generally
of poor quality, end with the sentence "This produces the results."
Authors, please put yourself in the shoes of the reviewer. On the
other extreme, there are artifacts that even produce LaTeX tables just
like they appear in the paper. This is great per se, but at the same
time, I need traceability.

***Suggestion:*** There should be a step-by-step walk through on how
   to get the paper's results.

## Documentation chaos

Perhaps facilitated by [mandating no less than five markdown
documents,](https://2020.esec-fse.org/track/esecfse-2020-artifacts)
many artifacts did not adhere to the submission guidelines
strictly. An abundance of information spread across a website, README,
and wiki, can be helpful later on, but adds to the confusion of the
reviewer. 

***Suggestion:*** Artifacts should have one canonical tutorial-style
   document for reviewers; additional information can be very helpful
   in practice and for later, but should be separate.

## GitHub is not a good platform for reviewing

Look at the chaos in the screenshot, which is from the official
ESEC/FSE artifact repository. As you can see, there are at least 5
different ways artifacts are stored there, and not all include the
paper number. Such accidental complexity needs to be removed.

![Chaos in the repository](/assets/posts/2020-06-26-repos.png)

GitHub has other issues, too. GitHub is not great in
1. enforcing consistency, or communicating quickly to the chairs which badges to award.
1. getting an overview of the state of your artifacts.
1. staying anonymous. Re-using your anonymous GitHub reviewer id (as suggested in the reviewing instructions) lets one draw conclusions on who is who, by matching anonymous ids with previous real-name committees, which are openly accessible on the web. GitHub facilitates this by showing when someone joined the service, even when other activity is hidden.


## And then there is always the nagging question of ...

> Wasn't this just a bitcoin miner in disguise with a static
  printf buried somewhere that outputs the results?

Despite putting lots of time into the artifacts track (over 25h!), I
would not be 100% confident in excluding this. Sure, I would be
negatively surprised, but can I rule it out? Honest answer: no.

***Suggestion:*** We need concrete guidelines for reviewers on how to
verify an artifact -- do I need to inspect the source code? Do I need
to be able to build it myself? Do I need to mutate the input such as
to observe mutated output (often times, verifying whether the output
is still correct is non-trivial, due to step functions, etc.)? Do I
need to verify all of the original results? Is a sample-based
evaluation enough?