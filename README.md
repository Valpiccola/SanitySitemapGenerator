# Sanity Sitemap Generator

## Overview

This tool is designed to automatically generate a sitemap powered by Sanity CMS with also the need to manage multiple languages.
It fetches data from Sanity CMS and constructs a sitemap XML file, which is essential for search engine optimization.

[Your final sitemap will look like this.](https://www.valpiccola.com/sitemap.xml)

## Features

- Fetches dynamic content types from Sanity CMS.
- Generates a sitemap XML file compatible with search engine requirements.
- Supports multilingual content for improved global SEO.

## Configuration

Before running the script, make sure to configure the following variables according to your specific requirements:
Adjust these settings in the script to match the specifics of your website and CMS setup.

### baseUrl: This should be set to the base URL of your website.

Example: const baseUrl = 'https://www.example.com';

### docTypes: This array should include all the document types from your Sanity CMS that you want to include in the sitemap.

Example: const docTypes = ["page", "business", "author", "blog", "event"];

## Compatibility and Considerations

### Sanity V3 and Internationalization

This tool is designed to operate seamlessly with Sanity V3 and is fully compatible with the latest version of the Sanity.

## Contributing

Contributions to enhance the tool are welcome. Please read our contributing guidelines before submitting a pull request.

## License

This project is licensed under the MIT License.
