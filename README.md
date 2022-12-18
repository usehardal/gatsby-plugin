# Hardal for Gatsby
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
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
      websiteId: "hardal_WEBSITE_ID",
      srcUrl: "https://usehardal.com/hardal.js",
      includeInDevelopment: false,
      autoTrack: true,
      respectDoNotTrack: true
    }
  }
];
```

## Configuration

- `websiteId` - Required. The website id of your hardal site
- `srcUrl` - Required. The url to the hosted `hardal.js`
- `includeInDevelopment` - Optional. Defaults to `false`
- `autoTrack` - Optional. Defaults to `true`
- `respectDoNotTrack` - Optional. Enables hardal respect Do Not Track feature. Defaults to `true`
