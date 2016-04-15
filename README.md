# jira-custom-css
Custom CSS for JIRA, to "condense" the layout

This is a simple CSS to customize the layout of JIRA 6.3, so that the information is more condensed.
The goal was to see more information on the screen, by avoiding wasted space :
- reduce the font size to 12px instead of 14px
- reduce the space between lines
- add a grey background to improve separation of the different zones of a detail view
- reduce the size of right column in detail view
- increase the size of form fields in creation view

Tested on JIRA 6.3.15 with Firefox, IE 9 and Chrome, on 1280x1024 screens
It has been reported NOT to work on JIRA Cloud instances (because they seem to escape HTML tags in the announcement banner)

Installation :
- Put the CSS file somewhere on the server (where it can be reached through HTTP)
- In the JIRA settings, enable the announcement banner, and put the following piece of code in it :
```html
<link href="/path/to/JIRA_condensed_style.css" rel="stylesheet" type="text/css" />
```

See https://answers.atlassian.com/questions/160863/jira-customize-css

Tip : if you modify the CSS and want to be 100% sure the browsers don't use on old cached version,
you can modify the CSS filename each time you modify it (for example with a date suffix)

This CSS is certainly not perfect : if you improve it, please let me know.
