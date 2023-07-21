---
title: Better Images in Astro
# slug being our url version of the title
slug: better-images-in-astro
excerpt: Last year, we published the first Astro image integration (@astrojs/image) alongside Astro 1.0. The goal was simple. Make image optimization effortless in Astro. Now, 1 year and 2.5 million downloads later, we’re ready to share our new vision for working with images in Astro. completely redesigned with new features, faster performance, and a better end-user experience with.
date: 2023-05-13
author: Erika and Fred Schott
---

Last year, we published the first Astro image integration (@astrojs/image) alongside Astro 1.0. The goal was simple: Make image optimization effortless in Astro.

Now, 1 year and 2.5 million downloads later, we’re ready to share our new vision for working with images in Astro: completely redesigned with new features, faster performance, and a better end-user experience with:

Automatic layout shift (CLS) prevention.
First-class Markdown, Markdoc & MDX support.
Integration with third-party services.
This new update will be available for all users starting in Astro 3.0, but you can opt-in today by setting the experimental.assets flag in your configuration file. You can also enable by passing the --experimental-assets flag to the Astro CLI.

How it works
From the start, we knew that we wanted an image API that felt as minimal as possible. We started with the original Component API from the @astrojs/image integration, and then built on it with a few new tweaks and changes.

But don’t let the minimal API fool you:

Astro optimizes your image using the modern WebP file format (by default).
For accessibility, the required alt prop helps improve your site for screen-readers and other tooling.
For even faster page-load performance, the loading and decoding attributes are added as defaults.
For the user experience, The width and height attributes are always included to prevent layout shift (more on this later).
Flexibility was another goal. We added the getImage() function to optimize an image in your project, on-demand, without using the component. Use this function to build your own custom Image component for any use-case you you have in mind.

Automatic layout shift prevention
Cumulative Layout Shift (CLS) is an essential metric to optimize for website performance. It is tracked as one of Google’s 3 Core Web Vitals and is weighted heavily in the Lighthouse performance score.

Astro’s new component automatically protects your site from layout shift. It works by inferring an explicit height and width for every image and including them in the generated tag. With explicit dimensions, the image can’t shift the page layout as it loads onto the page.

The output HTML is always a simple element, so you can also apply additional CSS styling for more advanced responsive layouts like fill and cover without risking layout shift.

Automatic Markdown & MDX support
One of the biggest improvements made over the original @astrojs/image integration is complete support for Markdown, Markdoc, and MDX. You can now reference images using a relative image path in your Markdown content or frontmatter, and Astro will automatically optimize them for you.

That’s it! Your stars.png image will be optimized automatically in the final HTML. You can also use the <Image /> component directly in MDX if you prefer for finer control over the image attributes, but in most cases the default settings will be enough to produce an optimized file size with a great image quality.
