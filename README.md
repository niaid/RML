# Welcome to the RML GitHub Page

- You can use the [editor on GitHub](https://github.com/niaid/RML/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

### Website pages
- [index.md](index.md) is our main homepage that publishes to [https://niaid.github.io/RML/](https://niaid.github.io/RML/) .  It has our schedule (I basically copied our poster).  **Please edit this file to add the link to your repo**.
- [listofrepos.md](listofrepos.md) is just the automatically populated list of our repos with their descriptions.  Originally, it was set up to automatically update based on the bcbb-training topic, but that seemed to mess other things up, so now it is just a manually made list.  The list is located in [_data/repos.yml](_data/repos.yml) .  You can add your repo to this file.
- Whenever you commit (and/or push) to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.
- You can edit these pages or add additional pages to the repo.


### Making a new Page

- If you want to make add a new page to the website, add it to the root of this repository.  There is an example of what the file should look like below.
- The Front matter is the section between the three dashes `---`.  This holds the variables used to build the page.  

  - If you add a *title* variable, then the page will appear in the sidebar of the site; otherwise it will not.
  - The *layout* variable can take 2 values, *default* or *post*.  These are the (you guessed it!) options for the page layout.  They are defined by the [minimal page theme](https://github.com/pages-themes/minimal) we are using. As far as I can tell, they are almost identical, except the post layout will automatically add the title at the top of the page, and if you include a date variable in the front matter, it will automatically add that as well.  
  - You can also design additional layouts, and put them in the [_layouts](_layouts) directory and use them in your front matter layout variable instead.

```markdown
---
title: Title of page
layout: default

---

[Link](url) and ![Image](src)

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text


```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).


### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/niaid/RML/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.  You can also [configure other settings](https://jekyllrb.com/docs/configuration/) in that file.


### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
