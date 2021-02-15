# BigCommerce Sitemap Generator
BigCommerce can automatically generate a single sitemap with up to 50k URLs. However, for stores with very large catalogs the 50k limit may not be high enough.

This node app will query your BC store's API to retrieve URLs for the following entities:
- Products
- Categories (TODO)
- Brands (TODO)
- Web Pages (TODO)
- Blog Posts (TODO)

The app creates multiple XML sitemaps, a sitemap index, then uploads them your store via WebDAV where Google can access the sitemap index.

## Usage
1. Make a copy of `.env.template` and name it `.env`
2. Fill in the API and WebDAV credentials. Note: The API keys need read-only access to Products and Store Content scopes.
3. Run `npm run dev`

## TODO
- Finish everything except Products
- Create a lambda deployment package script