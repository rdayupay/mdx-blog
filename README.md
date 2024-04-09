## MDX-based Blog

# Overview

This project is an interactive MDX-based blog using Next.js 14 (App Router).

You can view the live site [here](https://mdx-blog-rdayupay.vercel.app/).

![Screenshot of the final product](/docs/end-result.png)

## Technologies Used

- Next.js 14: Used as the main framework for building the project.
- React: Used for building user interfaces and components.
- MDX: Used for writing and rendering Markdown documents with embedded JSX components.
- Framer Motion: Used for implementing animations throughout the application.
- Bright: Used for syntax highlighting in code snippets.
- js-cookie: A simple, lightweight JavaScript API for handling cookies.
- rss: A library for generating RSS feeds.
- clsx: A utility for constructing className strings conditionally in JSX.
- date-fns: A library for manipulating JavaScript dates in a functional way.
- eslint: A tool for identifying and reporting on patterns found in ECMAScript/- JavaScript code.
- eslint-config-next: Official ESLint configuration for Next.js projects.
- gray-matter: A library for parsing frontmatter from markdown files.

## Getting Started

This is a Next 14 project. You'll first need to install NPM dependencies, and then run a local development server. Here are the relevant terminal commands:

```bash
# Install dependencies:
npm install

# Run a development server:
npm run dev
```

## Features Implemented

## 1. Homepage List of Posts

- Implemented a reverse-chronological list of blog posts on the homepage.
- Utilized a helper function to gather the list of blog posts.

![Screenshot showing the homepage with a reverse-chronological list of blog posts](/docs/homepage-list-of-posts.png)

---

## 2: Displaying MDX

- Rendered MDX content for each blog post dynamically.
- Used next-mdx-remote to handle MDX rendering.

![Screenshot showing the blog post layout with all of the content from the MDX file, with correct formatting (paragraphs, headings, etc)](/docs/blog-post-with-mdx.png)

---

## 3: Adding metadata

- Added metadata to the homepage and blog post pages for improved SEO.
- Leveraged Next.js Metadata API to specify site metadata.

```html
<title>Bits & Bytes</title>
<meta
  name="description"
  content="Discover JavaScript easily through our dedicated blog,…"
/>
```

And on the blog post page, it should look something like this:

```html
<title>Understanding the JavaScript Modulo Operator • Bits & Bytes</title>
<meta
  name="description"
  content="One of the most commonly-misunderstood operators…"
/>
```

---

## 4: Code Snippets with Bright

- Enhanced code snippet presentation with syntax highlighting using Bright.

![Screenshot of the code snippets with correct syntax highlighting](/docs/bright-syntax-highlighting.png)

---

## 5: Animated Division Widget

- Implemented a widget demonstrating the modulo operator with layout animations using Framer Motion.

![Screen recording showing the new behaviour, smooth layout animations](/docs/division-groups-animated.gif)

With remainder:

![Screen recording showing the final animation](/docs/divison-groups-demo-with-remainder.gif)

---

## 6: Circular Colors Widget

- Developed a widget demonstrating circular color selection based on a timer.
- Implemented functionality for starting, pausing, and resetting the timer.

![Screen recording of the `CircularColorsDemo` component](/docs/circular-colors-demo.gif)

This widget demonstrates how the Modulo operator can be used to select items from an array in a circular manner. A timer climbs from 0 to infinity, and that linear value is used to pluck one of three colors, circling back to the front on each 3rd value.

---

## 7: Dark Mode

- Implemented toggling between light and dark mode with theme persistence.

![Toggling between light mode and dark mode](/docs/dark-mode-toggle.gif)

---

## 8: RSS Feed

- Implemented an RSS feed for the blog to enable integration with RSS readers.

![Screenshot of the site header, showing the RSS icon](/docs/rss-icon.png)

---

## 9: Handling Invalid URLs

- Implemented a custom 404 page for handling invalid URLs.

![Screenshot of the 404 page](/docs/404-page.png)
