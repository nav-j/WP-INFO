## How to add products to our own created pages.

## **Option 1: Use WooCommerce Shortcodes (Recommended for beginners)**

WooCommerce comes with built-in **shortcodes** that you can add anywhere — in a **page**, **post**, or **block**.

### Example 1: Show all products

Just add this shortcode to your page (in a block or Classic editor):

```plaintext
[products]
```

That will display all published products, just like the shop page.

---

### Example 2: Show products by category

```plaintext
[products category="tshirts"]
```

(Change `"tshirts"` to your real category slug.)

---

### Example 3: Show specific products

```plaintext
[products ids="12, 34, 56"]
```

Use your product IDs (you can find them in **Products → All Products → Hover over a product**).

---

### Example 4: Show featured products

```plaintext
[featured_products per_page="8" columns="4"]
```

---

You can mix and match settings like:

```plaintext
[products limit="6" columns="3" orderby="date" order="DESC"]
```

 **How to use**:

* Go to **Pages → Your Page → Edit**
* Click the **“+”** icon → add a **Shortcode block**
* Paste the shortcode and update the page

That’s it!

---

## **Option 2: Use WooCommerce Blocks (if you’re using Gutenberg editor)**

If your site uses the **WordPress block editor**, you can visually insert product lists.

### Steps:

1. Go to **Pages → Edit your page**
2. Click the **“+”** → search for **“Products by Category”**, **“All Products”**, or **“Hand-picked Products”** block.
3. Choose the products or categories to show.
4. Update the page.

This method is easy and flexible with live previews.

---

## **Option 3: Use a Page Builder (Elementor, Divi, WPBakery, etc.)**

If you use **Elementor or Divi**, they have special WooCommerce widgets:

* In Elementor → drag “**Products**” or “**Woo Products Grid**” widget into your page.
* You can filter products by category, tag, or ID.

---

## Tip:

If you don’t want the default **Shop** page to show all products, you can:

* Go to **WooCommerce → Settings → Products → General**
* Under “Shop page,” change or deselect it — or
* Redirect `/shop` to your custom page.

---
