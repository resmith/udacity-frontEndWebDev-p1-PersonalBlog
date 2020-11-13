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

| - BlogList (entry point is index.html)
| \ BlogPost - by clicking on any article in the BlogList
_note_ - currently there is only the JS spread operator article
\ about - is in the footer, which is the bottom of the left column
\ credits - is in the footer, which is the bottom of the left column
| \ authors - enter by viewing an article and clicking on the author's name

## Page Structure

|-------------------- HEADER ---------------------------
| menu . . . ."
| menu content1 . content2"
| menu
| menu content3 . content4"
| menu
| menu content5 . content6 "
| footer ";

The page structure is defined in:

- for index.html it's defined in src/styling/blogListGrid.css using the Grid System
- for the other pages it's defined in src/styling/blogPostClasses.css using flexBox

Normally only one system would be used for defining the structure. Two were used to demonstrate knowledge of both.

## Directory Structure

| - Index.html (the entry point)
| \ src - the direcotry where the rest of the code is at
| \ authors - information on the authors for the articles
| \ posts - the posts
| \ styling - holds the CSS for the grids, flexbox and styling

## Notes

- To auto-refresh the page every 3 seconds during development, uncomment the following in index.html

```
   <meta http-equiv="refresh" content="3" />
```

- Used <link > for importing stylesheets instead of @import based on StackOverflow recommendation
  [Link vs import](https://stackoverflow.com/questions/10036977/best-way-to-include-css-why-use-import)
