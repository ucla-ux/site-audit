# Site audit

Performance and accessibility review to help design a better user experience

## Google Lighthouse

Google Lighthouse is an open-source, automated tool for improving the quality of web pages. It can be run in [Chrome DevTools](https://developers.google.com/web/tools/chrome-devtools) or installed locally and run from the command line.


- [Web Dev](https://web.dev/)
- [Google Pagespeed Insights](https://developers.google.com/speed/pagespeed/insights/)
- [Google Lighthouse](https://developers.google.com/web/tools/lighthouse)
- [Get Started using Lighthouse](https://developers.google.com/web/tools/lighthouse/#get-started)
- [Using Lighthouse on Chrome DevTools](https://developers.google.com/web/tools/lighthouse#devtools)
- [Using Lighthouse on command line](https://developers.google.com/web/tools/lighthouse/#cli)
---

## Cheatsheet

### Install

`npm install -g lighthouse`

See all options

`lighthouse --help`

To run an audit, use `--output` flags to export json, html or both. use `--view` to view report in browser.

`lighthouse https://mysite.ucla.edu --output html --view` 

`lighthouse https://mysite.ucla.edu --output html --output json --view`

`lighthouse https://mysite.ucla.edu --output html --emulated-form-factor=none --throttling-method=provided --view`

`lighthouse https://mysite.ucla.edu --output html --emulated-form-factor=none --view`

### Test on a site with authentication

When installed globally via `npm i -g lighthouse` or `yarn global add lighthouse`,
`chrome-debug` is added to your `PATH`. This binary launches a standalone Chrome
instance with an open debugging port.

1. Run `chrome-debug`. This will log the debugging port of your Chrome instance
1. Navigate to your site and log in.
1. In a separate terminal tab, run `lighthouse http://mysite.ucla.edu --port port-number` using the port number from chrome-debug.
1. ex. `lighthouse https://mysite.ucla.edu --port portnumber --output json --output html --view`

### View and share reports

- [Share repots online](https://developers.google.com/web/tools/lighthouse#report-viewer)
- [Share reports as JSON](https://developers.google.com/web/tools/lighthouse/#json)
- [Share reports as GitHub Gists](https://developers.google.com/web/tools/lighthouse/#gists)
- [Lighthouse viewer](https://googlechrome.github.io/lighthouse/viewer/)

Reports are saved in the directory command is run. If you want to output path to another folder use `--output-path`

ex: `lighthouse --output json --output-path <path/for/output.json>`

To view a report that's been saved as a Gist:

Add `?gist=<ID>` to the Viewer's URL, where `<ID>` is the ID of the Gist.

`https://googlechrome.github.io/lighthouse/viewer/?gist=<ID>`

Open the [Viewer](https://googlechrome.github.io/lighthouse/viewer/), and paste the URL of a Gist into it. Or upload the json file.

---

## Google links for study

- [Web Fundamentals](https://developers.google.com/web/fundamentals)
- [Design and UX Basics](https://developers.google.com/web/fundamentals/design-and-ux/ux-basics)
- [Auditing Performance](https://developers.google.com/web/fundamentals/performance/audit)
- [Accessibilty Basics](https://developers.google.com/web/fundamentals/accessibility)
- [Auditing Accessiblity](https://developers.google.com/web/fundamentals/accessibility/how-to-review)

---

## Accessiblity

- [Making the Web Accessible](https://www.w3.org/WAI/)

---

## Online Courses

- [Website Performance Optimization by Google](https://www.udacity.com/course/website-performance-optimization--ud884)


---

## Lighthouse reports

You can use this section to save reports and publish them on the web in this repo. 