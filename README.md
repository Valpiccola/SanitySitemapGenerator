# Sanity Sitemap Generator

## Overview

This tool is designed to automatically generate a sitemap powered by Sanity CMS with also the need to manage multiple languages.
It fetches data from Sanity CMS and constructs a sitemap XML file, which is essential for search engine optimization.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9" xmlns:xhtml="http://www.w3.org/1999/xhtml">
 <url>
  <loc>https://www.example.com/it</loc>
   <xhtml:link rel="alternate" hreflang="it" href="https://www.example.com/it"/>
   <xhtml:link rel="alternate" hreflang="en" href="https://www.example.com/en"/>
 </url>
 <url>
  <loc>https://www.example.com/en</loc>
   <xhtml:link rel="alternate" hreflang="it" href="https://www.example.com/it"/>
   <xhtml:link rel="alternate" hreflang="en" href="https://www.example.com/en"/>
 </url>
 <url>
  <loc>https://www.example.com/it/uno</loc>
   <xhtml:link rel="alternate" hreflang="it" href="https://www.example.com/it/uno"/>
   <xhtml:link rel="alternate" hreflang="en" href="https://www.example.com/en/one"/>
 </url>
 <url>
  <loc>https://www.valpiccola.com/en/one</loc>
   <xhtml:link rel="alternate" hreflang="it" href="https://www.example.com/it/uno"/>
   <xhtml:link rel="alternate" hreflang="en" href="https://www.example.com/en/one"/>
 </url>
</urlset>
```

## Features

- Fetches dynamic content types from Sanity CMS.
- Generates a sitemap XML file compatible with search engine requirements.
- Supports multilingual content for improved global SEO.

## Configuration

Before running the script, make sure to configure the following variables according to your specific requirements:
Adjust these settings in the script to match the specifics of your website and CMS setup.

### baseUrl

This should be set to the base URL of your website.
Example: const baseUrl = 'https://www.example.com';

### docTypes

This array should include all the document types from your Sanity CMS that you want to include in the sitemap.
Example: const docTypes = ["page", "business", "author", "blog", "event"];

## Compatibility and Considerations

### Sanity V3 and Internationalization

This tool is designed to operate seamlessly with Sanity V3 and is fully compatible with the latest version of the Sanity.

## Contributing

Contributions to enhance the tool are welcome. Please read our contributing guidelines before submitting a pull request.

## License

This project is licensed under the MIT License.
