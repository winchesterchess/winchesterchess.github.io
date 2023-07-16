The repo holds the source for the [winchesterchess.uk](https://winchesterchess.uk) website.

# To add a News post
1. Create an account on [github.com](https://github.com).
2. You can edit or add pages using a git client or online, start by editing [/_data/authors.yml](https://github.com/winchesterchess/winchesterchess.github.io/blob/main/_data/authors.yml) and adding a section for yourself. Your username will be the name without spaces on the first line of your section.
3. "Commit" the changes and open a "Pull Request", one of the site admins will merge it for you soon. You don't have to wait for this.
4. Make a [new page](https://github.com/winchesterchess/winchesterchess.github.io/new/main) and call it `_posts/YYYY-MM-DD-lower-case-title.md` (eg: `_posts/2023-07-15-summer-break.md`).
5. Paste in and edit this template:
   ```markdown
   ---
   layout: single # Don't change this
   title:  "Summer Break" # This is the page title, change it.
   date:   2023-07-15 19:01:00 +0100 # Make this the correct time you wrote the post
   author: bracken # This is your username from step 2
   categories: news # Don't change this
   tags: meetings # Add as many tags as you want
   ---
   <!-- Write your article here in "markdown" (https://www.markdownguide.org/basic-syntax/) -->
   ```
6. Commit and open a Pull Request as before, a site admin will merge the post soon.

# To add or change a different page
Adding or editing other pages on the site is similar, except they aren't in the `_posts` folder. Take `join.md` for example. You can just create new markdown files here and they will be available at `https://winchesterchess.uk/<page_name>`. The link in the navbar at the top of the site are in `_data/navigation.yml`.

# Previewing your changes
You can preview your changes on your computer if you have some programming skills. The site is a static site generated using [jekyll](https://jekyllrb.com/) and hosted in Github Pages, you should be able to render it by:
1. Have ruby >=v3 installed.
2. `gem install jekyll bundler`
3. `bundle exec jekyll serve --livereload`
4. Go to [http://127.0.0.1:4000](http://127.0.0.1:4000).
