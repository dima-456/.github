# Website initialization guide

In this walkthrough, you will learn the ways to set up your site to make sure it is visible to search engines, easy to find, and professionally displayed (having a thumbnail image and a favicon icon).

**Jump to**
- What is SEO?
- [Adding a site title](https://github.com/dima-456/.github/edit/main/profile/wesbiteinit.md#adding-a-site-title)
- [Adding a site description](https://github.com/dima-456/.github/edit/main/profile/wesbiteinit.md#adding-a-site-description)
- Adding a thumbnail image
- Adding a favicon
- Google analytics
- Miscellaneous best practices

## Adding a site title

Currently in your `index.html` file you should see a `<title>` element in your `<head>`.

```html
<title>Your Name Page</title>
```

This title tells the world what your website is. It should be between 50-60 characters. If this is my portfolio site, I would make my title look like this.

```html
<title>Anna Boone Portfolio</title>
```

If I'm working on my "About" page of my website, I need the page title to accurately reflect that. But just naming it "About" would limit the SEO on the page, and might be confusing with no other context. The recommended way to do solve this is to keep the homepage title and add the sub-page separated with a veritcal pipe or a slash. (For other pages, you would just change "About" to whatever the relevant keyword is.)

```html
<title>About | Anna Boone Portfolio</title>
```

## Adding a site description

Currently in your `index.html` file, you (most likely) do not have a site description in your `<head>`. To make sure our site is easy to find, we need to add one. 

```html
<meta name="description" content="Your site description">
```

This description will appear on Google and other search engines under the title. For instance, on this example, the title is "We asked for your Prince stories. Here's what you shared." and the description is "From quick brushes with him at First ave to being accused of stealing his pie."

![Screenshot of a news article preview on Google](https://github.com/user-attachments/assets/7758defb-8ca1-407c-86cf-ca6be582f50e)


Descriptions should be between **120-160 characters.** It should have some keywords that describe you and your work. Unlike the title, this description can be the same across all portfolio site pages. If you like, you can also adjust to each individual page.

Here's an example of what my site description would be. It contains keywords that are relevant to me ("visual journalist," "designing", "writing", etc., and includes my location. This example is 130 characters.


```html
<meta name="description" content="A visual journalist who wears many hats
(figuratively). Designing, developing, writing and editing for the Minnesota Star Tribune.">
```

## Adding a site description
