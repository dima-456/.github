# Creating mulitple pages for your portfolio sites

As you build your portfolio sites, you will need to create multiple pages (`work.html`, `about.html`, etc.). Here is detailed documentation on the two ways to do this, with the pros and cons for each.

**IMPORTANT:** No matter which way you create and link pages, each repository **must** have an `index.html` file. This file will be the homepage of your site, and the first thing people see when they visit your URL. Even if you want that page to highlight all your work, it must be named `index.html`, not `work.html` or something similar.

## 1️⃣ Linking HTML pages in the same repo

<table>
  <tr>
    <th>Pros</th>
    <th>Cons</th>
  </tr>
  <tr>
    <td>Only maintain  one repo</td>
    <td>Looks sloppier as a URL</td>
  </tr>
  <tr>
    <td></td>
    <td>Makes your repo larger</td>
  </tr>
</table>

Open your portfolio repo (`<username>.github.io`) in VS Code. Look at the folder explorer on the left sidebar (if you don't see this sidebar, click the file icon at the top left of the window — it looks like two pieces of paper stacked on top of each other).

<img width="394" height="423" alt="Screenshot 2026-04-19 at 6 01 03 PM" src="https://github.com/user-attachments/assets/1752d803-616b-4e41-8389-7dd17b826e63" />

In the image above, you can see I have an `index.html` file, a `styles` folder and an `images` folder. Now I want to create a new html file for my work page. To do so, I will right-click and hit "New file."

<img width="461" height="347" alt="Screenshot 2026-04-19 at 6 01 15 PM" src="https://github.com/user-attachments/assets/099baf44-b467-4909-bee8-65d664043a99" />

This opens a new file in my explorer. I name that file `work.html`, and now I can go into that blank file and add in all the normal html page structure I need.

<img width="404" height="332" alt="Screenshot 2026-04-19 at 6 01 30 PM" src="https://github.com/user-attachments/assets/06e408f0-87ff-493a-a5a4-cc90a08dd64a" />

I would recommend using the `starter-page.html` [in our helpful-code-snippets repo](https://github.com/dima-456/helpful-code-snippets/blob/main/html/starter-page.html) to set up the page with all the correct metadata and encoding.

With my `work.html` set up, I can now link to it from my other pages. For example, I can link to the work page in the navigation bar on my `index.html` file like so.

<img width="400" height="109" alt="Screenshot 2026-04-19 at 6 02 45 PM" src="https://github.com/user-attachments/assets/3d0bfc7e-1998-4887-bc80-c234cbb6de24" />

______________________________________________

## 2️⃣ Creating new Github Pages repos to link to

<table>
  <tr>
    <th>Pros</th>
    <th>Cons</th>
  </tr>
  <tr>
    <td>Looks cleaner as a URL (url/work) instead of url/work.html)</td>
    <td>Have to maintain multiple repositories</td>
  </tr>
  <tr>
    <td>Can keep relative images in each page’s repo</td>
    <td></td>
  </tr>
</table>

Go to our [example-page](https://github.com/dima-456/example-page) template repository and **click the "Use this template" green button** in the top right corner (not the green "Code" button!).

<img width="1381" height="455" alt="Screenshot 2026-04-19 at 6 41 27 PM" src="https://github.com/user-attachments/assets/800d58fb-c15f-44f5-a8d9-76164fbd59a1" />

When you click the button, you will see two options. You want to then select "Create a new repository."

<img width="265" height="116" alt="Screenshot 2026-04-19 at 8 19 40 PM" src="https://github.com/user-attachments/assets/d2ddd8c6-b665-46d3-88d2-dac52eb9b5ba" />

When you select this option you will then see the typical page you see when you create a new repository. There are a couple important steps here.

1. Make sure that the owner of the repository is you, and not the `dima-456` organization.
2. The name of this repository will become the URL page name. For instance, if I name my repository "work," then the page link will be `<username>.github.io/work`.

<img width="844" height="326" alt="Screenshot 2026-04-19 at 8 20 00 PM" src="https://github.com/user-attachments/assets/53d836d2-e183-4207-adfc-84460fac5bd8" />

When you are redirected to the new repository on the Github website, click the "Settings" button on the far right of the menu bar.

<img width="1288" height="164" alt="Screenshot 2026-04-19 at 11 01 30 PM" src="https://github.com/user-attachments/assets/2729f9d4-9789-4ce5-9b45-06387d409ade" />

Once you are in the settings, click the "Pages" button at the bottom of the "Code and automation" section.

<img width="352" height="661" alt="Screenshot 2026-04-19 at 11 01 47 PM" src="https://github.com/user-attachments/assets/576fa99f-abf7-463a-8eb4-b1898005c8b6" />

Under the Branch section, select "main" and then save. 

<img width="830" height="454" alt="Screenshot 2026-04-19 at 11 01 57 PM" src="https://github.com/user-attachments/assets/4408ab47-f0c4-49e7-ad8b-2fffc85524e6" />

It may take a few minutes for the cache to break, but once it does you will be able to see this new repo live at `<username>.github.io/<repo-name>`.

From here, you can clone the repo locally and work in it just like you work in any of the other repos. 

**Don't forget**
1. Don't clone the repo locally *into* your portfolio site repo. Make sure it lives outside of your `<username>.github.io` folder.
2. The `styles` folder is empty. You will need to create a new `style.css` file in this folder to add your css for this page.
3. You might have base styles in your `<username>.github.io` that you want applied to this repo as well. You can call in that repo's stylesheet to your new Github Page repo by adding this link above the `</head>` in your `index.html` file.
`<link href="https://<username>.github.io/styles/style.css" rel="stylesheet">`






