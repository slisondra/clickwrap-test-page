# Clickwrap test page

This project includes three HTML files, index.html, login.html 
and site.html.

There is no application server for the files. The 
[GitHub pages](https://pages.github.com/) feature is used to
serve the pages. 

[View the test page and form](https://docusign.github.io/clickwrap-test-page).

## index.html
The index.html file is a form to collect Clickwrap parameters. It makes a
GET request on the **login.html** page. Since there is no 
application server, parameters are passed using the 
fragment (#) string.

### The Clickwrap parameters
1. **Environment hostname** The hostname section of the DocuSign environment
   used for your account.

   Available from: your Clickwrap code popup window.

3. **Account ID** The DocuSign account for your Clickwrap.

   Available from: your Clickwrap code popup window.

3. **Clickwrap ID** The id of your Clickwrap.

   Available from: your Clickwrap code popup window.

## login.html
An example login page for a name and password. For this example,
the password is ignored. When the login button is clicked,
the page's JavaScript combines the clickwrap settings from
the prior page with the form's `name` setting, and calls
the clickwrap JavaScript SDK. 

After it returns success, the JavaScript loads the home page
of the site, `site.html`

## Using the test page
1. Fill in the form, and click the button `Show the example login page`
1. Fill in the login form (the password is optional), and click
   `Login`

**Remember** that the agreement ceremony is only shown once per 
Login Name (used for the ClientUser ID parameter). 
To show the agreement ceremony again, either 
change the Name on the login page or update the Clickwrap settings
on DocuSign.

## Support, Contributions, License

Submit support questions to [StackOverflow](https://stackoverflow.com). Use tag `docusignapi`.

Contributions via Pull Requests are appreciated.
All contributions must use the MIT License.

This repository uses the MIT license, see the
LICENSE file.
