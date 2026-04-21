# Website initialization guide

In this walkthrough, you will learn the ways to set up your site to make sure it is visible to search engines, easy to find, and professionally displayed (having a thumbnail image and a favicon icon).

**Jump to**
- What is SEO?
- [Adding a site title](https://github.com/dima-456/.github/edit/main/profile/wesbiteinit.md#adding-a-site-title)
- [Adding a site description](https://github.com/dima-456/.github/edit/main/profile/wesbiteinit.md#adding-a-site-description)
- [Adding a thumbnail image](https://github.com/dima-456/.github/edit/main/profile/wesbiteinit.md#adding-a-thumbnail-image)
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

## Adding a thumbnail image

My site is looking good and I'm ready to share it with the world now. But when I go to text it to my friends, it looks like this. 

![Screenshot of a link sent via text with no image](https://github.com/user-attachments/assets/2b453e33-3563-4703-9049-b4e22e6284cd)

My site title is there, so that's good. But on the whole, this isn't a link that would encourage a click. And it's not just messaging — sharing this link on social media would result in the same treatment. To make our link more visually appealing and to encourage people to click into our site, we need to add a thumbnail iamge.

```html
<meta property="og:image" content="image-link-here">
```

Adding this line of code in the `<head>` of our `index.html` (or other page) will give our site a thumbnail image representation, which will give us better click-through rates. 

Currently throughout your site, you probably have image links referenced like this: 

```html
<img src="images/catkeyboard.webp">
```

This is called a relative path. Your code is looking for a folder at the same level as the HTML file called `images`, going into that folder and finding the file named `catkeyboard.webp`

For our thumbnail image, we need an absolute path. To find the absolute path, you will simply add your portfolio site URL in front of the relative path. 

Add the thumbnail image you want to your images folder, and then make sure you have committed and pushed your repo. Now you should be able to visit https://**username**.githbub.io/images/**thumbnail**.webp and see that image in your browser. (Your username and your thumbnail image file name will be unique to you.)

If so, you are good to copy that URL and place it between the quote marks in the `content=""` spot of the meta tag.

Some things to note:
- WebP formats are accepted, which means you can have an animated image as your thumbnail if you want.
- A variety of sizes can be supported, but a good starting place is 1200px x 650px. You could go up to a 3:4 or 2:3 ratio if you want a little more visual impact.
- This image can vary page to page, or you can use the same image across all pages.
- If you have created a logo for your site, that would be a good image option.

I'm going to use my cat keyboard gif as my thumbnail image, so this is what I am adding to my site.

```html
<meta property="og:image" content="https://annaboone.github.io/images/catkeyboard.webp">
```

Now I can text all my friends my portfolio site and they can see a cat typing away, enticing them to click!

![Screenshot of a link sent via text with a thumbnail image]([https://github.com/user-attachments/assets/2b453e33-3563-4703-9049-b4e22e6284cd](https://github.com/user-attachments/assets/1543f98a-c5ee-4ba9-a9e6-7c04fab0dff6))

