# Paperless Inspector Transaction Emails

This is the template for transactional emails coming out of Paperless Inspectors.
The emails are fully responsive and support all major email clients (not a small feat).

## Getting Started

This uses Zurb's Foundation for Emails framework to create responsive emails
with support for all the major email clients. It automatically inlines all CSS
and uses Inky to help alleviate the endless nesting of tables in the design.

### Prerequisites

This is a bit tricky, as Zurb hasn't kept up maintanence of Foundation for
Emails. I've personally found it best to first install Windows Subsystem for 
Linux, which you can find here: 

https://docs.microsoft.com/en-us/windows/wsl/install-win10

From there, you'll want to install the Node Version Manager:

https://github.com/creationix/nvm

Use this to install the long-term support version of Node (v5.6.0 at this time)

### Install

Once you've done that, move into bash and clone this repository. In the folder
it created, run

```
npm install
```

This will take some time to build all the dependencies. There are countless 
opportunities for error here. You may need to make sure you install the
`python-minimal`, `make`, and `g++` packages in Ubuntu. 

## Running the Template Engine

To start a server and build the templates, simply run:

```
npm start
```

This will start up a server at http://localhost:5000 that you can use to
design the templates.


## Building the Final Templates

Run this command to build the final HTML output of the template:

```
npm run-script build
```


## Deployment

This repository uses [Netlify](https://netlify.com) as a static site host. It
watches this repository for changes and automatically builds the site for you.

The site can be found at https://paperless-inspectors-emails.netlify.com/


## Built With

* [Foundation for Emails](https://foundation.zurb.com/emails/email-templates.html)
* [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10)
* [NVM](https://github.com/creationix/nvm)
* [Node](https://nodejs.org)