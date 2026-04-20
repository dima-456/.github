# Creating mulitple pages for your portfolio sites

As you build your portfolio sites, you will need to create multiple pages (`work.html`, `about.html`, etc.). Here is detailed documentation on the two ways to do this, with the pros and cons for each.

**Note: ** No matter which way you create and link pages, each repository **must** have an `index.html` file. This file will be the homepage of your site, and the first thing people see when they visit your URL. Even if you want that page to highlight all your work, it must be named `index.html`, not `work.html` or something similar.

## 1️⃣ Linking HTML pages in the same repo

<table>
  <tr>
    <th>Pros</th>
    <th>Cons</th>
  </tr>
  <tr>
    <td>
      1. Only maintain  one repo
    </td>
    <td>
      1. Looks sloppier as a URL<br>
      2. Makes your repo larger</td>
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

## 1️⃣ Creating new Github Pages repos

<table>
  <tr>
    <th>Pros</th>
    <th>Cons</th>
  </tr>
  <tr>
    <td>
      1. Only maintain  one repo
    </td>
    <td>
      1. Looks sloppier as a URL<br>
      2. Makes your repo larger</td>
  </tr>
</table>

