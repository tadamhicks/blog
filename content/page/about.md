---
title: "About Me"
date: 2023-01-17T15:19:45-05:00
url: "/about/"
draft: true
---

Who am I, anyway? What does it mean to be me? What does it mean to be?

Spend a few minutes with me and you will realize that no matter how many years I put between myself and my philosophy studies as an undergraduate, I am and always will be a philosopher.

According to Encyclopedia Brittanica, “philosophy” comes from the Greek word, philosophia, which means “love of wisdom.” Although my better half frequently points out that with every year I age I lose a little more of my sensibility, one might consider this an accomplishment in the pursuit of balance! Perspective is my ultimate goal, and I try to apply the practice to life itself and all the things within it.

Like most people on the planet I spend a lot of my time working. I made a concerted effort throughout my life to pursue work that aligns well with my talents, my values, and my passions. Though some days one of these legs doesn’t feel as true as others, I am generally very fortunate to be able to make a living the way that I do. I work as a Field CT for a burgeoning software company that helps customers with digital transformation, datacenter and cloud automation, as well as DevOps.

This blog will have aspects of both of the above facets of my life, as I use my philosophical nature to help pursue professional wisdom and share it with my customers and partners. Sometimes I will get very tactical, and sometimes I may stray into hobbies such as my passion for coffee or my passion for whisk(e)y.

A smattering of details on my professional and academic background here:

# Morpheus Data

## Field CT
### 01/2020-Present

## Sr. Solutions Architect
### 01/2017-01/2020

Leadership: Player coach for small, 5 man team with a mission to reduce time-to-value of a complex, hybrid cloud orchestration solution. Doubled company revenue by creating incredible stickiness through simplifying Morpheus rollouts. Technical: Wrote Jenkins workflow libraries, Ansible installer for Morpheus, Ansible modules for Morpheus, Python libraries for Morpheus, Golang based log aggregator and analysis pipeline for new customers, contributions to Go SDK for Morpheus Terraform Provider, and Terraform blueprints for cloud infra maintenance. Evangelism: Launched our APAC business through training sessions with partner and customer technical resources. Assisted in the realization of our EMEA arm through trainings and partner/customer consults. Contributed several white papers, blogs and conducted speaking engagements to evangelize DevOps and Morpheus. Performed over three dozen complete implementations of Morpheus at customer sites spanning 3 years. Internal DevOps: Co-architected Morpheus integration with PowerDNS, Chef, Ansible, SaltStack and Puppet. Architect and administrator for company SPF/SCVMM/HyperV cloud. Wrote demo Groovy on Grails/MySQL application, Django application and dotNET application for Sales Engineering team’s use. Crafted demos using Terraform, Chef, SaltStack, Ansible and Puppet within Morpheus and all clouds for Sales Engineering team. Configured and administered Morpheus for all cloud integration, public and private, for company production use as well as for sales use. Administrator for company production Morpheus to manage internal application infrastructure. PowerDNS architect and admin and Active Directory Administrator. Wrote automation framework for installer builds using Python/Flask, Jenkins Pipeline and custom Groovy scripts for http requests. Manage build/release via Jenkins EC2 slaves and s3/CloudFront for package repos. Wrote custom Chef recipe for CI/CD pipeline for Morpheus Application installation. Wrote CI/CD demo with Docker build/deploy to kubernetes and Morpheus for bespoke Python/Django application.

# SquareTwo Financial

## Systems Engineer II
### 07/16-01/17

## Enterprise Applications Engineer
### 04/15-07/16

My big accomplishment at SquareTwo was creating a tool called Hawkeye. Since this is a blog and not a resume I’ll tell it as a story:

I joined S2 with wide open eyes to the world of Enterprise IT. I may be putting words in my leaderships' collective mouths, but I believe they liked my can-do attitude, my mathy nature (more on that later), and my passion for the python programming language. One of their engineers and my hiring manager had written metric tons of python for automation, monitoring and reporting and they seemed eager to have someone on board who could support and expand the tools and reduce their dependency on one human. For those in the industry it was a company that felt a lot like the one written about in The Phoenix Project, and in TPP terms they were trying to reduce their “Brent” problem.

Starting out I was paired with a mentor, to whom I still owe an incredible amount of gratitude (Greg if you ever read this just know you made an impact), and the big, shared burden that was being pushed toward me was managing the biweekly release or production code from the software team. We ran Oracle for almost everything. We had SOA middleware with WebLogic, we had the ADF product, and of course the databases were Oracle. The other items we handled releases for were Informatica and Autosys. Releases were very traditional IT releases where all changes that needed to be accounted for/promoted into production were tracked via spreadsheet that was versioned and stored in JIRA. The Friday before a release weekend we would conduct a meeting with a representative from these teams to go through the changes and make sure we understood them, and then on Sunday we would have our scheduled outage and run through the release. Releases for the production software, called Eagle, included a build as we weren’t yet using an intermediary for build like Hudson/Jenkins. This came later and dramatically reduced our release times and created a great deal of repeatability in a critical part of the process.

Rather than belabor the slow attempt toward “DevOpsification” of this process I want to shift gears towards other items at this org that became quickly more interesting and challenging. To understand the challenge a bit of background:

Though it may leave some people with a sense of “ew” the organization I worked for was in the business of debt reconciliation. While SquareTwo itself was not a debt collector, it served a network of debt collection firms. There are a lot of complexities that don’t serve this story as it relates to my background, but part of what we did for these firms was provide software for pursuing collections from debtors as well as deep analytics and debt portfolio acquisitions.

The relevant part of this background is that when dealing with American citizens' credit there is actually an enormous amount of regulatory oversight and compliance is both difficult and critical. Coming off the heels of the recession there was an overarching theme of anger toward what were being called “Predatory Lenders” and The Obama Administration had taken concerted efforts to force any organization that was in the business handling debt to be more dilligent about their processes. To us that meant increased scrutiny on the media/documentation we had associated with a debt account so as to avoid inadvertent harassment of individuals whose debt we had purchased in the pursuit of collections.

Media and documentation is really what this is all about. Mountains of it. Disorganized, poorly formatted, highly irregular, and yet completely essential. So important was documentation, and validating that we had compliant amounts of it on a debtor before we contacted them, that we spun up an entire team to sort through it. But humans are humans, and eventually these humans with this nearly insurmountable task in front of them found themselves in front of potential failure unless IT could help them with some organization. Enter me.

So the first thing the business asked for was just a simple way of looking at media as it related to a customer account and indicating if it met certain criteria. Our development organization was under immense pressure for critical features, and the production side of IT owned the media itself, so it fell to my team. In rapid fashion we spun up a small development effort and crafted a tool that would interact with the production database and render account data and its media in one easy UI. It had a prescriptive flow that allowed operators to move quickly through stacks of accounts.

I owe a lot of thanks to my team, but since this is my story I’m going to bang my own drum here, and say that I developed most of it myself. My team had much more intimate knowledge of the data architecture, so they were critical in helping me identify which data to touch and use, and how to work with it. Nigel, Martin, and Eric, if you guys ever read this I will forever be in your debt!

Having learned a lot about our media and our accounts, the business came back with a new requirement: do this for millions of accounts in six months. The manual, eyes-on process was not going to cut it, and management approached me and asked if it would be possible to automate it. I did some fast evaluation of open source OCR libraries, looked back at my math and Python notes from the past and realized that at least in theory it would be possible to extract text from the documents, embedded jped/png or otherwise, and run it through some ML a la scikit-learn and achieve classification results that would meet the regulatory requirements we had for media validation. My concern was about scale.

I was quickly thrust into a few vendor meetings as we solicited some of our partners in the space, but was non-plussed by what I saw. Being a software shop serving a captive network in a niche industry, my management and I thought it would be cool even if really hard to pull off to build it ourselves. When I voiced my scaling concerns a VP in the org introduced me to Hortonworks, and I sat in one of the most compelling meetings I’ve ever been in with one of the smartest people I’ve ever met. Shane Kumpf instantly understood the problem domain and explained that while his stack wasn’t the solution it was certainly a framework for scaling it that could help, and we could use to expand upon and do so much more. And that’s how I became a Hadoop guy!

The next six months were dizzying as I worked with some consultants to quickly refactor my mathy framework writtin in Python to leverage Apache Spark. Because the API did not support the ML modelling I wanted to use in Python, I also had to switch to writing it all in Scala. This is what IT people live for, truth be told…I felt like Maverick from Top Gun as I furiously coded a powerful but small application and hacked some functionality on external dependencies into this incredible tool for performing massively parallel, distributed computation. It was the nerd highlight of my young life!

As this “Hawkeye” application started to bear fruit (and trust me there were some failed launches that caused many involved endless ulceritis), we moved to harden it by building a team beneath it to do ongoing care and feeding. I used my passion for automation and DevOps to build a nice pipeline for the platform, and started handing more and more of the daily concern over until I left the org. It was a doozy, but so worth it and incredibly gratifying. I wish every young IT upstart the opportunity for such a challenge.