# HOW TO ADJUST PRODUCT SIZE IN ELEMENTOR SHORTCODE WIDGET

---

##  **Step 1: Insert the Shortcode Widget**

1. Open your page with **Elementor**
2. Click the “+” to add a new section
3. Drag a **Shortcode** widget into the section
4. Paste your WooCommerce shortcode, e.g.:

   ```plaintext
   [products ids="12,34,56" columns="3" limit="6"]
   ```
5. Click **Update**

---

##  **Step 2: Adjust Product Columns & Count (via Shortcode)**

WooCommerce shortcodes have built-in layout controls.
Here are the most useful ones:

| Parameter | Example          | Description                |
| --------- | ---------------- | -------------------------- |
| `columns` | `columns="3"`    | Number of products per row |
| `limit`   | `limit="6"`      | Total products to show     |
| `orderby` | `orderby="date"` | Order by newest first      |
| `order`   | `order="DESC"`   | Sort direction             |

**Example:**

```plaintext
[products category="furniture" limit="6" columns="3" orderby="date" order="DESC"]
```

➡️ This will make the products appear in **3 columns** across, which adjusts their size automatically.

---

##  **Step 3: Adjust Product Image Size (Global WooCommerce Setting)**

Since Elementor’s Shortcode widget simply outputs WooCommerce HTML, product image sizes are controlled by WooCommerce itself.

1. Go to **WordPress Dashboard → Appearance → Customize**
2. Click **WooCommerce → Product Images**
3. Change:

   * **Main image width**
   * **Thumbnail width**
   * **Thumbnail cropping**
4. Click **Publish**

Now your shortcode products will resize accordingly.

---

##  **Step 4: Add Custom CSS (Optional, for precise control)**

If you want to make them *exactly* the size you want, you can add a custom class to your Shortcode widget and style it.

###  Add a CSS class in Elementor:

1. Click your **Shortcode widget**
2. In the **Advanced tab → CSS Classes**, type:

   ```
   custom-products
   ```

###  Then add this CSS:

You can place it in:

* **Elementor → Custom CSS** (if you have Elementor Pro), or
* **WordPress → Appearance → Customize → Additional CSS**

```css
/* Adjust WooCommerce product grid inside Elementor shortcode */
.custom-products ul.products li.product {
  width: 30%;           /* Product card width */
  margin: 1.5% auto;    /* Spacing between products */
}

.custom-products ul.products li.product img {
  height: 250px;        /* Control image height */
  object-fit: cover;    /* Crop neatly */
}

.custom-products ul.products li.product .woocommerce-loop-product__title {
  font-size: 16px;      /* Adjust product title size */
  text-align: center;
}
```

💡 This CSS works **only for that widget** because you added the `custom-products` class.

---

## **Bonus Tips**

* Use `columns="4"` for smaller cards (more per row)
* Use `columns="2"` for larger product cards
* Combine with Elementor section padding to create a balanced look

---
 **Summary**

| Method                 | What it Controls               | Where to Apply              |
| ---------------------- | ------------------------------ | --------------------------- |
| `columns` / `limit`    | Number & layout of products    | In shortcode                |
| WooCommerce Customizer | Image dimensions               | Appearance → Customize      |
| Custom CSS             | Card width, image height, text | Elementor or Additional CSS |

---
