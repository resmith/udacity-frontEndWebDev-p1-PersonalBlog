# udacity-frontEndWebDev-p1-PersonalBlog

## Installation Instructions

```
git clone <thisRepo>
cd <toTheDirectoryTheRepoIsIn>
click the index.html file so it opens in a browser
```

The application should now be working
_Note:_ this is a static HTML site and requires no web server

## Application Flow

```
| - BlogList (entry point is index.html)
| \ BlogPost - by clicking on any article in the BlogList
_note_ - currently there is only the JS spread operator article
\ about - is in the footer, which is the bottom of the left column
\ credits - is in the footer, which is the bottom of the left column
| \ authors - enter by viewing an article and clicking on the author's name
```

## Page Structure

The oveall page structure is defined in src/shared/pageGrid.css

```
      "header header header"
      ".      .      . "
      "menu   .      content"
      ".      .      ."
      ".      footer footer "
      ".      .      .";

```

_Note:_ The content is the same but placement varies depending on screen size to create a responsive layout.

Each pageType then defines it's own grid or flexbox within the content. For example, the blogPost defines the content within blogPostGrid.css as:
grid-template-columns: 80vw;
grid-template-rows: 5vh 5vh 65vh 8vh;
grid-template-areas:
"title"
"author"
"article"
"buttons";

## Directory Structure

```
| Index.html (the entry point)
| \ src - the directory where the rest of the code is at
|   \ authors - information on the authors for the articles
      \ css - css styling for the author content

|   \ blogList - the posts
      \ css - css styling for the blogList (index.html)

|   \ blogPosts - holds the CSS for the grids, flexbox and styling
      \ css - css styling for the blogPosts (index.html)

|   \ shared - holds shared code / assets
      \ css - css styling used by multiple categories


```

## Notes

- To auto-refresh the page every 3 seconds during development, uncomment the following in index.html

```
   <meta http-equiv="refresh" content="3" />
```

- Used <link > for importing stylesheets instead of @import based on StackOverflow recommendation
  [Link vs import](https://stackoverflow.com/questions/10036977/best-way-to-include-css-why-use-import)
