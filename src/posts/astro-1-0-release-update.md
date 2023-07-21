---
title: Content for Everyone
slug: astro-1-0-release-update
excerpt: How Astro Helped Contenda Build a Content-Sharing Platform in One Month
date: 2023-29-06
author: Astro Team
---

Contenda, an artificial intelligence company that came onto the scene in 2021, has been building towards the ambitious goal of making content for everyone. Their vision starts with being a catalyst for developer advocates by making repurposing content easy for a variety of mediums.

Developer advocates are the bridge between software companies and their developer users, often creating content to help educate and raise awareness in the community about particular features. Contenda makes it possible to take, for example, a video tutorial and turning it into a blog. This saves time and can even make it easier for a cross-functional team to collaborate.

When Contenda needed to share draft blog posts publicly with other people, they turned to Astro and Netlify as their solution. This combination of technologies let them stay laser focused on their goal of making collaboration and content creation easy.

Take any video and turn it into effective written content with Contenda.
Challenges
Contenda is a team of less than 10 people. They often need to share blogs with each other in order to address pain points and conduct reviews but they couldn’t do these things without sharing their emails and API keys with one another. This also posed a security problem for customers that they knew they had to solve eventually. To resolve these issues for internal and external users, Contenda created Share Pear, an open-source tool for quickly sharing Markdown blog post previews.

Requirements
Share Pear needed to be built without requiring backend changes since Contenda did not want to overload themselves by managing additional complexity. Ideally, it also needed to be cost-effective but preferably free.

In addition to meeting their requirements, the main benefit of choosing Astro was its flexibility. With Astro, popular JavaScript frameworks like React are available, but optional. A site can be built using just HTML, CSS and, if necessary, vanilla JavaScript. This enables team members with less web development experience, such as product designers and content authors, to edit and maintain the site often without any developer intervention required.

Cassidy (Contenda CTO) saw an opportunity to pair Astro with Netlify’s on-demand builders. Astro was the obvious choice because it had a component that both natively supported Netlify’s builders and rendering markdown to HTML. It also helped that Contenda had previously chosen Astro for their main marketing website so the technology was familiar enough for the rest of the team to jump in.

Solution and Implementation
Contenda found success in Astro’s developer community. The team was able to enlist the help of the core team and active contributors in Astro’s community Discord server. From there, building Share Pear moved quickly.

This was my first time using Astro. I would say, getting started with Astro was simpler than other frameworks. It felt like the onboarding time was way smoother and especially the docs are so up-to-date that it’s a 1-to-1 match with your code sometimes.
