---
title: API Reference

language_tabs:
  - json: JSON
  - xml: XML

toc_footers:
  - <a href='https://remix.mashery.com/member/register'>Sign Up for an API Key</a>
  - <a href='http://bestbuyapis.github.io/bby-query-builder/#/productSearch' target="_blank">Query Builder</a>

includes:
  - products
  - categories
  - recommendations
  - errors

search: true
---

# Overview

Welcome to the Best Buy Developer API site! Whether you're an API pro, a beginning developer or a Best Buy partner, our extensive API catalog is waiting for your imagination. Our API suite allows you to query <a href="https://developer.bestbuy.com/documentation/products-api" class="inline-link">Products</a>, <a href="https://developer.bestbuy.com/documentation/stores-api" class="inline-link">Stores</a>, <a href="https://developer.bestbuy.com/documentation/reviews-api" class="inline-link">Reviews</a> and much more. Come on in to explore our data, browse descriptions of the available attributes and see examples of working requests and responses.

If this is your first time using our APIs, please check out our Getting Started guide. If you already have your API key, our Search and Response Formats can help you refine your search or results.

# Authentication

```md
[#request]:

http://api.bestbuy.com/v1/stores(region=ut)?format=json&show=storeId,city,region&apiKey=YourAPIKey
```

```md
[#response]:
```
```json
{
  "from": 1,
  "to": 10,
  "total": 10,
  "currentPage": 1,
  "totalPages": 1,
  "queryTime": "0.002",
  "totalTime": "0.007",
  "partial": false,
  "canonicalUrl": "/v1/stores(region=\"ut\")?format=json&show=storeId,city,region&apiKey=YourAPIKey",
  "stores": [
    {
      "storeId": 1402,
      "city": "American Fork",
      "region": "UT"
    },
    {
      "storeId": 773,
      "city": "Orem",
      "region": "UT"
    },
  ]
}
```

> Make sure to replace `meowmeowmeow` with your API key.

Kittn uses API keys to allow access to the API. You can register a new Kittn API key at our [developer portal](http://example.com/developers).

Kittn expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: meowmeowmeow`

<aside class="notice">
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>






