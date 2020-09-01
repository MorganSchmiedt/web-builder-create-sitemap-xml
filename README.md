## Web Builder Module - Create sitemap.xml file

This module allows the [@deskeen/web-builder](https://github.com/deskeen/web-builder) engine to create a `sitemap.xml` file.

## Install

```
npm install @deskeen/web-builder
npm install @deskeen/web-builder-create-sitemap-xml
```

### Usage

And add the module to the list of modules: 

```javascript
const builder = require('@deskeen/web-builder')
const builder.build([
  source: [
    // List of files or directories
  ],
  modules: [
    [
      '@deskeen/web-builder-create-sitemap-xml',
      {
        urls: [
          // List of website URLs
        ],
        path: '/sitemap/path', // Path where sitemap.xml file will be created
        filename: 'sitemap.xml', // Optional filename. Defaults to "sitemap.xml"
      }
    ]
  ]
])
```
