# ethereumdefensealliance-com
This is the source code for https://ethereumdefensealliance.com, a site for a group of advocates promoting long-term network health.


**Table of Contents**

- [Local Development](#local-development)
- [Directory Structure](#directory-structure)
- [Editing Existing Content](#editing-existing-content)



---



## Local Development

1. Clone the repo
1. Install dependencies: `bundle install`
    - Ruby may need to be installed first if not already packaged with your OS
1. Create a feature branch off of the `main` branch (`git checkout -b new-branch-name`)
1. Start the local server: `bundle exec jekyll serve`
1. Go to <http://localhost:4400/> to view changes

To build the site, use `bundle exec jekyll build`.

Resources:

- [Jekyll Docs](https://jekyllrb.com/docs/)
- [Liquid Syntax](https://shopify.github.io/liquid/basics/introduction/)



## Directory Structure

- root - Contains site pages
- `_data` - Contains data files, such as resources
- `_includes` - This folder is [designated by Jekyll](https://jekyllrb.com/docs/includes/) for files that can be "included" into other files
    - `components` - Contains reusable non-content components, including the html head, nav, and footer
    - `partials` - Contains sections of page-soecific content
- `_layouts` - Contains layout templates used to build pages
- `_plugins` - Contains custom [Jekyll plugins](https://jekyllrb.com/docs/plugins/), which have usage instructions at the top of each file
- `assets` - Contains js, css, images, and files



## Editing Content

To find the content you want to edit, first visit the markdown page in the root folder. Some content is directly in this file, like with `404.md`. Other content like the index (homepage) is pulled in from `_includes/partials/index/` for ease of maintenance.

Some sections that use data files include members and delegates. That data can be found in `_data/`.




