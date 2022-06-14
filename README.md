# Overview
## Jekyll Structure
### _includes
Partials used to create components that can be included on pages. Things like footers, headers, analytics, social links, etc. These are not rendered at a top level.

These are used by inserting `{%- include <filename>.html -%}`

### _layouts
Layouts that can be reused across multiple pages. Provides the scaffolding for page content to be inserted into.

These are used by inserting `layout: <filename>` in the frontmatter of a page.

### _config.yml
The place to put any config values that can be accessed through:

`{%- site.<value> -%}`

## Content
### _drafts
A place to track unpublished articles.

### _posts
The actual content of the site. These will be enumerated in chronological order on the index.

### Top Level Markdown Files
Top level files like `index.markdown` and `about.markdown` translate to paths on the website. `index` will translate to the top level root path. Any other