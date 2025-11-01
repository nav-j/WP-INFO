## **About the Shortcode**

```plaintext
[products ids="12, 34, 56"]
```

### What it does:

It displays **only the specific products** whose IDs you list — for example, product IDs **12, 34, and 56**.

Each product will show with:

* Product image
* Title
* Price
* Add to Cart button
  ...exactly like they appear on your WooCommerce shop page.

---

## **How to Use in Elementor**

1. Edit your page with **Elementor**.
2. In the left panel, search for **“Shortcode”**.
3. Drag the **Shortcode widget** to where you want the products to appear.
4. Paste your shortcode:

   ```plaintext
   [products ids="12, 34, 56"]
   ```
5. Click **Update** and **Preview** the page on the front-end.

 **Note:** Sometimes Elementor’s editor doesn’t show a live preview of shortcodes — but it **will display correctly** when you view the published page.

---

## **How to Find Product IDs**

1. Go to **WordPress Dashboard → Products → All Products**
2. Hover your mouse over a product name
3. You’ll see the product ID under the name — e.g., *ID: 34*

---

## **Pro Tips**

* You can show as many product IDs as you want:

  ```plaintext
  [products ids="10, 12, 15, 18"]
  ```
* You can also combine this with layout controls:

  ```plaintext
  [products ids="12, 34, 56" columns="3" orderby="date"]
  ```
* Works with both **Elementor Free** and **Pro**.
* Fully compatible with caching, pagination, and WooCommerce themes.

---

 **Final Answer:**

> Yes, `[products ids="12, 34, 56"]` works perfectly in Elementor’s **Shortcode widget** — just make sure the IDs are correct and the products are published.

---
