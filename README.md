<p align="center">
  <a href="https://usehardal.com/?utm_source=github&utm_medium=gatsby_plugin_logo" target="_blank">
    <img src="https://res.cloudinary.com/raufsamestone/image/upload/v1671398927/hardal/gj5urlgigxm9axbpp1oh.svg" alt="Hardal" width="180" height="84">
  </a>
</p>

# Hardal for Gatsby

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![version](https://img.shields.io/badge/version-1.0.1-green.svg)](https://semver.org)

An official plugin to add the [Hardal](https://usehardal.com/) tracking snippet to your [Gatsby](https://www.gatsbyjs.com/) site.

## Install

`npm install --save gatsby-plugin-hardal`

or

`yarn add gatsby-plugin-hardal`

## How to use

```javascript
// In your gatsby-config.js

plugins: [
  {
    resolve: `gatsby-plugin-hardal`,
    options: {
      websiteId: "<PASTE_YOUR_WEBSITE_ID>",
      srcUrl: "https://app.usehardal.com/hardal.js",
      includeInDevelopment: true,
      autoTrack: true,
      builtInEvents: false, // get your built-in events like scroll, rage click, etc.
      respectDoNotTrack: true,
      eventModel: "web2" // web3 is coming soon!
    }
  }
];
```
