# FJ Production

Premium responsive storefront for FJ Production. Orders are sent directly to WhatsApp; there is no checkout or payment gateway.

## Adding the owner's catalog

The catalog is populated with the owner-supplied product names, prices, categories and image filenames. To add or edit a product, edit `products` at the top of `app.js` and use only owner-provided values:

```js
{
  id: 'unique-id',
  name: 'Exact product name',
  price: 'PKR exact price',
  category: 'Exact category',
  description: 'Owner-provided description',
  image: 'path/to/owner-image.jpg'
}
```

The catalog automatically enables search, category/price filters, lazy-loaded images, and pre-filled WhatsApp order links. Keep image files inside the repository (for example `assets/products/`) and do not add unsupported product claims, reviews, certifications, discounts, prices, or imagery.

Run locally with:

```bash
python3 -m http.server 4173
```
