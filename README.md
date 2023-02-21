# pawsey-poster-site

Supporting site for the [Pawsey 2023 summer internship showcase event](https://pawsey.org.au/event/2023-summer-internship-showcase/).

## Run locally

Requirements: [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and [Hugo](https://gohugo.io/installation/)

Clone the repo with its submodules:

```shell-session
git clone --recurse-submodules https://github.com/megascrapper/pawsey-poster-site
```

Change directory:

```shell-session
cd pawsey-poster-site
```

Run Hugo:

```shell-session
hugo serve
```

Then open the specified address in a browser (hint: look at the line that says something like `Web Server is available at http://localhost:1313/pawsey-poster-site/ (bind address 127.0.0.1)`)

Refer to [Hugo documentation](https://gohugo.io/documentation/) for more information on how to use Hugo.

## Development

### Directory structure

| Path                              | Description                                                 |
| --------------------------------- | ----------------------------------------------------------- |
| `content`                         | Page source in Markdown, one page per file.                 |
| `content/_index.md`               | Source for the main page                                    |
| `assets`                          | Image files                                                 |
| `static/plot-data`                | Plotly plot data in JSON format                             |
| `static/pawsey_poster.pdf`        | Poster file                                                 |
| `layouts/partials/head-last.html` | HTML code to be appended at the end of each page's `<head>` |
| `shortcodes/load-plotly.html`     | Shortcode for loading `plotly.js` to the page               |
| `shortcodes/plotly.html`          | Shortcode for placing Plotly plots                          |
| `shortcodes/nootstrap-table.html` | Shortcode for making bootstrap tables look a little nicer   |

### Theme

This site uses Paige theme by [Will Faught](https://github.com/willfaught) It handles general layout and configuration of the site. At the time of writing this, it uses commit `b462632` of the theme. Please see the [theme documentation](https://github.com/willfaught/paige/tree/b4626326f963a3d5604afd14fde99b103569019d) for more details.

### Bibliography

`hugo-cite` is used to handle references and bibliography on the main page. Commit `ca42411` is used at the time of writing. Refer to [the documentation](https://github.com/loup-brun/hugo-cite/tree/ca4241165ffe541b3b59137c8d8e9dea1226a7e8) for details.

## Plotly

Plotly shortcodes are taken from <https://ig248.gitlab.io/post/2018-11-05-plotly-sample/> and are located in `shortcodes/load-plotly.html` (loader) and `shortcodes/plotly.html` (plot).

## Deployment

Deployed via GitHub Pages.
