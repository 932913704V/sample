---
id: tutorial-docusaurus
title: Building a website using Docusaurus
---

## What is  Docusaurus?

⚡️ Docusaurus will help you ship a beautiful documentation site in no time.

🧐 Docusaurus is a static-site generator. It builds a single-page application with fast client-side navigation, leveraging the full power of React to make your site interactive. It provides out-of-the-box documentation features but can be used to create any kind of site (personal website, product, blog, marketing landing pages, etc).

## Fast Track (Installation) ⏱️

### Step 01 :
Download and install a suitable IDE for you. (Recommend : Visual studio code.    VS code).

### Step 02: Create Git Account.

Git is a version control system for tracking changes in source code during software development and it can help you synchronise and version files between your local system and your online repository. Git for Windows includes Git Bash, a terminal application. If not already installed, see Installing Git.
  
### Step 03: Download and Install Node.js :
Node.js version >= 14 or above (which can be checked by running node -v). You can use nvm for managing multiple Node versions on a single machine installed.
When installing Node.js, you are recommended to check all checkboxes related to dependencies.
Check that you have the minimum required version installed by running the following command:

 ```
 node -v
 ```

You can see version larger than Node 8.

![](../../../../static/img/tutorial/Docusaurus_node_version.jpg)

### Step 04:  Install Yarn (Optional)
We highly recommend that you install Yarn, an alternative package manager that has superb performance for managing your NPM dependencies. Check it out here.
Check that you have the minimum required version installed by running the following command:
 ```
 yarn -v
 ```

You  can see a version  as follows:

![](../../../../static/img/tutorial/Docusaurus_yarn_version.jpg)

### Step 05: Create a GitHub repository and local clone

follow the link for working with git. [Click the link](tutorial-git.md)

### Step 06: After Cloning the web site Install the Website using following command. 

```
$ yarn
```
For Local development

```
$ yarn start
```
This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

#### The website will be running on localhost
Our development server locally, so we're running the website on localhost at port :3000

```
http://localhost:3000/
```

### Step 07: How to change Images, Nav bar, footer, sidebar, and docs on local site.

#### Nav bar : WEBSITE-DOCUSAURUS-SKELETON → docusaurus.config.js

![](../../../../static/img/tutorial/Docusaurus_navbar_img.jpg)

Under themeConfig there is a section called Navbar using that user can change navigation bar items as follows:
```
Tittle  : ‘Name of your Ministry’

Logo    :	alt: ‘Name of your Ministry’

            src: ‘source location of your logo’(img/srilanka_logo.png)

ITems   :   to: Location of about us page (Docs/ about-us)

		    Label: Display name of nav Item -( ‘About Us’)

		    Position: Position of the item it can be left, right or center - (’left’)
```
 
You can change the navigation bar item names and positions as you like as mentioned above.


#### Footer : WEBSITE-DOCUSAURUS-SKELETON → docusaurus.config.js

![](../../../../static/img/tutorial/Docusaurus_footer_img.jpg)

At the end of themeConfig page there is a section called footer using that user can easily change footer items.


#### Side bar : WEBSITE-DOCUSAURUS-SKELETON → sidebars.js

![](../../../../static/img/tutorial/Docusaurus_side_bar_fe.jpg)

![](../../../../static/img/tutorial/Docusaurus_side_bar.jpg)

```
About-us-slidebar:

type:   ‘Category’

Label:  Name of desire nav Item - (About us )

Items:  locations of markdown files, [‘About-us/about-us’, ‘about-us/the-officials’]  same way you can change all the sidebar items.
````

#### Docs: WEBSITE-DOCUSAURUS-SKELETON → docs

![](../../../../static/img/tutorial/Docusaurus_docs.jpg)

##### Docs Folder: 
This contains folders such  as about-us, contact -us and Institutions, inside those relative  Markdown files are there. Users can change the files as they wish.

#### Tips: Structure of The website

```
C:website-mot-gov-lk
├───.docusaurus
├───blog
├───docs
|    ├──────about-us
|    |     └───about-us.md
|    |     └───the-officials.md
|    ├──────contact-us
|    |     └───contact-us.md
|    ├──────institutions 
|          └───1-DRP.md
├───i18n
│   ├───si
│   └───ta
├───src
│   ├───components
│   ├───css
│   └───pages
└───static
|
├── docusaurus.config.js
├── package.json
├── README.md
├── sidebars.js
└── yarn.lock
```
- /blog/ - Contains the blog Markdown files. You can delete the directory if you've disabled the blog plugin, or you can change its name after setting the path option. More details can be found in the blog guide.

- /docs/ - Contains folders such  as about-us, contact -Us and Institutions, inside those relative  Markdown files are there. Customise the order of the docs sidebar in sidebars.js. You can delete the directory if you've disabled the docs plugin, or you can change its name after setting the path option. More details can be found in the docs guide.

- /i18n/ - This folder contains sinhala and tamil translated markdown files, Images, etc .

- /src/ - Non-documentation files like pages or custom React components. You don't have to strictly put your non-documentation files here, but putting them under a centralised directory makes it easier to specify in case you need to do some sort of linting/processing.

- /src/pages - Any JSX/TSX/MDX file within this directory will be converted into a website page. More details can be found in the pages guide.

- /static/ - Static directory -  contains an img (Image) folder,  inside that having all the images of the web site. 

- /docusaurus.config.js - A config file containing the site configuration. 

- /package.json - A Docusaurus website is a React app. You can install and use any npm packages you like in them.

- /sidebars.js - Used by the documentation to specify the order of documents in the sidebar.

### Step 07: Website Internationalization (I18N)

It is easy to translate your website with  internationalization (i18n) support.
Automatic locale detection or translation not offered in I18n. for more detail [Click Here](https://docusaurus.io/docs/i18n/introduction)

__I18n file structure__

```
/i18n/
├───si
│   ├───docusaurus-plugin-content-blog
│   ├───docusaurus-plugin-content-docs
│   │   └───current
│   │       ├───about-us
│   │       ├───contact-us
│   │       └───institutions
│   ├───docusaurus-theme-classic
│   └───img
│       ├───ta
│       │   └───img
│       │       └───tutorial
│       └───tutorial
└───ta
    ├───docusaurus-plugin-content-blog
    ├───docusaurus-plugin-content-docs
    │   └───current
    │       ├───about-us
    │       ├───contact-us
    │       └───institutions
    ├───docusaurus-theme-classic
    └───img
        ├───img
        │   └───tutorial
        ├───si
        │   └───img
        │       └───tutorial
        ├───ta
        │   └───img
        └───tutorial
```

01. All the English medium files are inside of the docs folder namely  about us, contact us, Institutions. So, you can edit all the markdown files as you want. 
To convert content of those files into sinhala medium, copy all the English medium files and  paste them to - i18n\si, use following code:

```
cp -r docs/** i18n/si/docusaurus-plugin-content-docs
```
Now you can simply erase all English medium contents and replace them with sinhala medium content. Also you must copy all the images from website-docusaurus-skeleton\static\img to sinhala folder i18n\si\img. 
Do the same thing to Tamil Language, Use following code.

`````
cp -r docs/** i18n/ta/docusaurus-plugin-content-docs 
`````
Or
if you are not delete or add new markdown files to docs folder You can just edit the insides of  i18n/si/docusaurus-plugin-content-docs markdown files for Sinhala and to Tamil language you can change  i18n/ta/docusaurus-plugin-content-docs markdown files.
