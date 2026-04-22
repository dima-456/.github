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

![Screenshot of a link sent via text with a thumbnail image](https://github.com/user-attachments/assets/2a3c68f8-37ef-4789-9f9d-73bab53e58e1)

## Adding a favicon

Now I can send people my full link and they can open my portfolio site. Yay! When they do, they see my site title in the tab next to a gray globe. That globe is called a favicon, and that's the default option. But I don't like that, and it doesn't represent my site very well, so let's change it!

![Screenshot of the tab with no favicon](https://github.com/user-attachments/assets/c0b96353-6e5e-46ba-9e88-b49288012dac)

Your favicon is set in the `<head>` of your html page, just like the site description, title, and thumbnail image we have set up. The most common favicon ico format is a `.ico`, which is an atypical format. To get it, we need to take a few steps.

First, we need to create the favicon. This is going to appear super small on your website, so you want it to be as simple as possible. An intial, an emoji, or a small icon will work best.

Create your image on a square canvas no larger than **48 by 48 pixels.** Export your image as a .png.

Now that our image is created, we are going to convert to a favicon using an online converter. [This is the one I use](https://www.icoconverter.com/) but you may find one you like more. There is also a Photoshop extension to save as a .ico. 

A note if you use the link I sent above: These are the settings I use. **Make sure you hit the "Convert" button, and NOT the download buttons below (those are ads).**

![Screenshot from the favicon icon converter](https://github.com/user-attachments/assets/aafb4edb-8038-49eb-84d2-3c1e32ef4b01)

Move your new .ico file into your `images ` folder in your portfolio repo. From here, we can add it to our site `<head>  `. 

```html
<link rel="icon" href="your-image-path" type="image/x-icon">
```

I named my favicon "anna_favicon.ico" and placed it into my images folder. So this is the code I am using in my `<head>`:

```html
<link rel="icon" href="images/anna_favicon.ico" type="image/x-icon">
```

Now when I go to my site, I see my favicon in the tab next to my site title. Nice!

![Screenshot from the favicon icon converter](https://github.com/user-attachments/assets/6a9d0ff1-0874-4eaf-b2b6-fcadbef61986)
