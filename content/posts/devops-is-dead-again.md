---
title: "Devops Is Dead, Again!"
date: 2018-11-19T14:20:06-05:00
draft: true
tags: ["devops", "technology"]
categories: ["devops", "technology"]
---

DevOps has died once more

One, quick Google search for “DevOps is dead” will yield pages of blogs dedicated to the untimely demise of what was once IT’s much heralded cult-religion.  The idea that Developers and Operations personnel could work together in sharing responsibilities for agile feature development AND stability is admirable.  However, the skillset and mentality required has pushed the tools available from “shared responsibility enablement” starkly into “shift left” territory.

Spend time at any conference and it quickly becomes apparent that “DevOps” has turned into a euphemism for infrastructure-as-code.  Kubernetes, collectively referred to as k8s, has become a de facto standard for this model in the last 1-1.5 years.  Underlying infrastructure, the real metal and pipes, is still in the nearly cold, dead hands of the operations team.  But, upon the shiny tin we have watched an evolution occur starting with virtualization on through to containerization and now clustered container scheduling that reduces the day-to-day need for this team.  Now developers can self-serve within abstracted virtual and containerized environments not just compute, but storage and even networking.  The entire operational config lives as code.

There is still a problem, though: most critical applications are still run in virtual machines.  So, while the development teams throughout the Enterprise are learning how to think about defining infrastructure elements in simple ways as a component of automating the setup of their applications, when code is pushed to production changes to the environment are still in the hands of many individuals to be performed manually.

“But there’s a good reason!” the bench of infrastructure people decry.  This writer will concede that checks and balances, auditability and subject-matter-expertise sound like good reasons on paper.  When you step back a bit, though, there’s no reason that any of these so-called reasons can’t be automated.  One of the main challenges to accomplishing this is that the CI environment has stopped looking like the production environment.  Organizations claiming full CI/CD have either fully modernized their production world to look like dev (think k8s) or have completely latched on to orchestration throughout all of their environments.

So, while DevOps seems to be a waning philosophy, and the IT business leaders are scratching their heads to make sense of the religion they have been pushing, a new form of developer has emerged: The Infrastructure Automation Engineer.  These individuals spend their days in code editors much like their developer siblings, but instead of writing business logic they are writing infrastructure automation logic.  They traverse multiple languages, and much of their “code” is actually declarative for system APIs, triggered by events within the code of the traditional application developer.

One of the reasons I joined Morpheus Data nearly two years ago was because I was tired of fielding the interviews to fill “DevOps Engineer” roles on “DevOps Teams.”  The term had lost its meaning to me, a once passionate believer in the high movement.  Morpheus presented me with an opportunity to stand on a soapbox and preach to the new zeitgeist lurking in the Enterprise.

In fact, when I first looked at the product that I now stand behind I had an uncanny feeling that it would unseat DevOps.  “It’s DevOps in a box!” proclaimed a colleague, and if a way of behaving can be encapsulated as a tool, then surely that way is indeed philosophically dead.

What I see now from my unique, privileged position is that organizations are trying to evolve, to embrace infrastructure automation engineering as a critical component of application delivery, to go post-DevOps…but the sprawling toolset is formidable and frequently results in a spaghetti system of overlapping necessities.  Morpheus represents a tremendous leap forward in this regard, as the approach of our team is to standardize across the board in an agnostic fashion, and alleviate the burden of tool sprawl and self-wrought automation scripting.

DevOps is dead!  Long live post-DevOps!