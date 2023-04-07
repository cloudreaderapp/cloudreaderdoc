---
title: How to customize your site?
section: Configuration
order: 4
---


## Customize your site

### File layout

The template is based on the following files.

| Directory                | Content                                                             |
| :----------------------- | :------------------------------------------------------------------ |
| docs                     | The documents for your site                                         |
| doc/docs.json            | A predefined file used by eleventy to generate the site left menu   |
| doc/quick-start-guide.md | A predefined file for the home page                                 |
| _data                    | The directory that host the site configuration file `metadata.json` |
| _includes                | The eleventy template and  nunjucks page layout                     |
| _site                    | The static html pages ready to be publish                           |
| src                      | some static assets used in the template                             |
| node_modules             | node.js dependencies                                                |

You can start your site customization by modifying the file `_data/metadata.json`
Then, simply add your mardown files in `/doc`

### Site customization

#### Site wide configuration

| Option                  | Content       | Usage                                                                            |
| :---------------------- | :------------ |----------------------------------------------------------------------------------|
| title                   | string        | Site title you can use in your markdown page with {{ metadata.title }} shortcode |
| supportEmail            | string        | Mail used int the in main page **Talk to us** link.                              |
| titleMenu               | string        | Left Top Menu title, better with single word                                     |
| search                  | true or false | Work in progress ...                                                             |
| headerButtonContactUs   | true or false | If true, swap the default `Edit this page` button to `Contact Us` button         |

 

#### Git repo configuration used for 'Edit htis page'

| Option                  | Content       | Description                                        |
| :---------------------- | :------------ |----------------------------------------------------|
| gitRepo                 | string        | Url to your repo like https://github.com/per1/11ty |
| gitEdit                 | string        | Url path for edit mode : "edit" for github         |
| gitBranch               | string        | Git branch : "main" for github                     |

`gitEdit` and `gitBranch` can tuned to adjust your remote git provider url pattern.
The final **Edit this page** url is build with: {{gitRepo}}/{{gitEdit}}/{{gitBranch}}/docs/{{your-page.md}}



#### Main page configuration'


| Option                  | Content       | Description                                    |
| :---------------------- | :------------ | ---------------------------------------------- |
| quickStartIntro         | string        | Main page tag line (3rd line)                  |
| quickStartShowVideoTour | true or false | If true, display the Hero block                |
| heroTitle               | string        | Hero Title                                     |
| heroDescription         | string        | Hero description                               |
| heroImage               | string        | Hero image url                                 |
| heroUrl                 | string        | Hero image link                                |
| quickStartQuickLinks    | true or false | If true, display the 4 Quick link cards        |
| ctaText                 | string        | Quicklink sub-title                            |
| cardHead`1234`          | string        | Card Title                                     |
| cardDesc`1234`          | string        | Card sub-titl                                  |
| cardLink`1234`          | string        | Carl link, can link page or external links     |

Should the cards link to some of your pages, start to create them first, then update the url.



