# jira-custom-css
Custom CSS for JIRA

This is a simple CSS to customize the layout of JIRA 6.3.
The goal was to see more information on the screen, by avoiding wasted space :
- reduce the font size to 12px instead of 14px
- reduce the space between lines
- reduce the size of right column in detail view
- increase the size of form fields in edit view
- etc

Tested on JIRA 6.3.15 with Firefox, IE and Chrome.

Installation :
- Put the CSS file somewhere on the server (where it can be reached through HTTP)
- In the JIRA settings, enable the announcement banner, and put the following piece of code in it :
<LINK href="http://jiraserver/path/to/jira-custom-css.css" rel="stylesheet" type="text/css">

See https://answers.atlassian.com/questions/160863/jira-customize-css
