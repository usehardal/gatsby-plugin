<p align="center">
  <a href="https://usehardal.com/">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://imge.usehardal.com/cdn/logo/new/svg/o9vnmleauvr2t5xvn9xe.svg?raw=1">
      <source media="(prefers-color-scheme: light)" srcset="https://imge.usehardal.com/cdn/logo/new/svg/yglazyhcy7kv6053lrso.svg?raw=1">
      <img src="https://imge.usehardal.com/cdn/logo/new/svg/yglazyhcy7kv6053lrso.svg?raw=1" alt="Hardal" width="180">
    </picture>
  </a>
</p>

# Hardal for Gatsby

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE) [![version](https://img.shields.io/badge/version-1.0.3-green.svg)](https://semver.org)

Add the Hardal tracking snippet to your [Gatsby](https://www.gatsbyjs.com/) site with this plugin.

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
      eventModel: "web2"
    }
  }
];
```
