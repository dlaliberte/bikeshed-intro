# Introduction to Writing Specifications with Bikeshed

- [Introduction to Writing Specifications with Bikeshed](#introduction-to-writing-specifications-with-bikeshed)
  - [Meta](#meta)
  - [Overview](#overview)
  - [Installing Bikeshed](#installing-bikeshed)
    - [Using GitHub](#using-github)
  - [Initial setup](#initial-setup)
  - [Starting Templates](#starting-templates)
  - [Sample Full Specifications following Best Practices](#sample-full-specifications-following-best-practices)
  - [Spec writing overview](#spec-writing-overview)
    - [Explainer to Specification](#explainer-to-specification)
  - [Strategies for incremental development](#strategies-for-incremental-development)
  - [Other Intros](#other-intros)
    - [Not specific to Bikeshed](#not-specific-to-bikeshed)

## Meta

- This document: [Introduction to Writing Specifications with Bikeshed](https://dlaliberte.github.io/bikeshed-intro/index.html)
- Source: [bikeshed-intro/index.md at updates · dlaliberte/bikeshed-intro](http://go/gh/dlaliberte/bikeshed-intro/blob/updates/index.md)
- Issues: [Issues · dlaliberte/bikeshed-intro](http://go/gh/dlaliberte/bikeshed-intro/issues)

## Overview

This document is intended as a simple introduction to writing specifications of web APIs using Bikeshed.  Very extensive [Bikeshed Documentation](https://tabatkins.github.io/bikeshed/) is available, but it is a complex tool which is a challenge to get started using since there is a lot to learn before one can become productive.

As the Bikeshed documentation says: "Bikeshed is a spec-generating tool that takes in lightly-decorated Markdown and spits out a full spec, with cross-spec autolinking, automatic generation of indexes/ToC/etc, and many other features."

So the goal here is to help beginners get started using Bikeshed in the simplest way possible. And then we provide some guidance for start writing the first few revisions of a specification.  We only cover the basics for many topics and refers to other documents for more complete details.  The following topics are covered here:

- Installing Bikeshed - There are multiple ways to use it, but we recommend installing it to run locally.
- Using GitHub for your specification repository, with initial empty specification source file.
- Strategies for how to incrementally develop your specification.


## Installing Bikeshed

The [Bikeshed Documentation: Installation](https://tabatkins.github.io/bikeshed/#installing) provides details on  several different ways for how to install and run Bikeshed.  We recommend you install it on a local machine so you can run it multiple times as you make changes to the specification.

- Make sure you have Python 3.7 or later.
- Install Bikeshed with pip3, if you can.
  - `pip3 install bikeshed`
  - `bikeshed update`
- Alternatively, you can use pip or pipenv, but see details at: [Bikeshed Documentation - Installing Bikeshed Itself](https://tabatkins.github.io/bikeshed/#install-final)
- You don't need to install "Bikeshed for Development", unless you are planning to do development on Bikeshed itself.


### Using GitHub

Assuming you will be using GitHub to develop and provide public access to your specification, you should first decide whether you will create a new repo or use an existing repo.  Either way, you will then want to do the following:

- Enable GitHub Pages
- Create an initial "empty" specification file, spec.bs or index.bs.
  - e.g. [Minimal template](http://go/gh/WICG/starter-kit/blob/main/templates/index.bs)
- Set up the following files which will cause GitHub to automatically process any updates to the specification file by testing whether Bikeshed can regenerate the html.
  - ... See [Spec Prod Documentation](https://w3c.github.io/spec-prod/)



## Initial setup

[Domenic's guide to spec excellence - Docs](http://doc/1cRVD1k-hDBGfLVwTG14P_ZqJLM4d5-Z4vpwYFb_4qks#heading=h.qc07m2oa0jm)
(mostly tactical "how to start a new spec")

## Starting Templates

Different types of APIs could have specs that follow different patterns.  Here is a list of several:

* [Minimal template](http://go/gh/WICG/starter-kit/blob/main/templates/index.bs)
* ...



## Sample Full Specifications following Best Practices

* [Navigation API](https://wicg.github.io/navigation-api/)
* [Prioritized Task Scheduling](https://wicg.github.io/scheduling-apis/)
* [Close Watcher API](https://wicg.github.io/close-watcher/)



## Spec writing overview

### Explainer to Specification

[How to read, write, and think about specs - Slides](http://go/how-to-specs#slide=id.p)

## Strategies for incremental development

If your API code already exists, and you have WebIDL specifications for that code, a great place to start is to copy in a subset of the WebIDL that corresponds to the public API.

After that, then you can add infra specs that reference the WebIDL specs.


If you have an implementation...

If you don't have an implementation...


Citing and linking.

Infra vs webidl

## Other Intros

A very helpful document, by Gary Kac, similar in purpose to this one:
[Writing Procedural Specs](https://garykac.github.io/procspec/)

### Not specific to Bikeshed

[Writing Promise-Using Specifications](https://www.w3.org/2001/tag/doc/promises-guide)

[Draft Spec - Read Write Web Community Group](https://www.w3.org/community/rww/wiki/Draft_Spec)

[QA Framework: Specification Guidelines](http://go/w3cstd/qaframe-spec/)

[Chromium Specification Mentors](http://go/chromium-spec-mentors)

[Home | Internet-Draft Author Resources](https://authors.ietf.org/)

[Web Platform Design Principles](https://w3ctag.github.io/design-principles/)
