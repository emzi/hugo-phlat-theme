## RTL'ed Hugo-Phlat-Theme
\- This repository contains rtl version of the Phlat theme. It's originally a [@nraboy](https://github.com/nraboy) work.

\- Contents are converted from Markdown to HTML manually by [Hugo](http://gohugo.io/) static site generator. You can host your static site on [Github Pages](https://pages.github.com/), [GitLab Pages](https://pages.gitlab.io/), Bitbucket (via [Aerobatic](https://www.aerobatic.com/)) and others.

![screenshot_rtl](https://cloud.githubusercontent.com/assets/1899175/15530309/e109eddc-2268-11e6-9346-b578ee8cc4c6.png)

### Installation

    hugo new site my-blog
    cd $_
    git clone git@github.com:emzi/hugo-phlat-theme-rtl.git themes/hugo-phlat-theme-rtl
    mv -f themes/hugo-phlat-theme-rtl/exampleSite-rtl/* .
    hugo server --buildDrafts

---
### Posts
- Each post must be located in `content/post`
- A post should be started with the below snippet (called 'frontmatter') at the beginnig:

        +++
        author = "Author"
        categories = [ "Category" ]
        date = "YYYY-MM-DDThh:mm:ss+03:30"
        description = "Description"
        draft = true/false
        tags = [ "tag1", "tag2" ]
        title = "Title"
        +++

    `YYYY-MM-DD` should be in Gregorian date. `hh:mm:ss` refers to time and don't touch `03:30` which is [Iran UTC time offset](https://en.wikipedia.org/wiki/UTC%2B03:30). You may also see `04:30` that is because of detected summer clock on author's OS.
    When you are still working on your post, set the `draft` as `true`. Once completed, ensure it’s no longer a draft: `hugo undraft content/post/<file-name>.md` or simply replace 'true' with 'false'.

- Put images in `static/img` directory.

\+ [Read More](https://github.com/emzi/hugo-phlat-theme-rtl/blob/master/READMORE.md)
