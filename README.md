<p align="center">
  <a href="https://usehardal.com/">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://imge.usehardal.com/cdn/logo/new/svg/hnav0hronsb1fttdnmph.svg?raw=1">
      <source media="(prefers-color-scheme: light)" srcset="https://imge.usehardal.com/cdn/logo/new/svg/ptlior6hfvknmblekenh.svg?raw=1">
      <img src="https://imge.usehardal.com/cdn/logo/new/svg/ptlior6hfvknmblekenh.svg?raw=1" alt="Hardal" width="180">
    </picture>
  </a>
</p>

# Hardal for Gatsby

Add Hardal analytics to a [Gatsby](https://www.gatsbyjs.com/) website by loading the Hardal tracking script through `gatsby-config.js`. The plugin configures the website ID, script URL, automatic tracking, built-in events, and Do Not Track behavior.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE) [![Package version](https://img.shields.io/badge/version-1.0.3-green.svg)](package.json)

## Getting started

You need a Gatsby site, a Hardal website ID, and a compatible Hardal tracker URL. Install the plugin, then add the configuration below to your Gatsby project.

## Installation

```bash
npm install --save gatsby-plugin-hardal
# or
yarn add gatsby-plugin-hardal
```

## Configuration

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

`includeInDevelopment` controls whether the script is included during development; production builds include it automatically. See [the plugin source](src/gatsby-ssr.js) for the exact script attributes.

## Support

Maintained by [Hardal](https://github.com/usehardal).

- [Hardal documentation](https://docs.usehardal.com)
- [Report an issue](https://github.com/usehardal/gatsby-plugin/issues)
- [Hardal website](https://usehardal.com)

