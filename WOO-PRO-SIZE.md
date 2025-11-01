## **If You’re Using WooCommerce Shortcodes**

When you insert products via shortcode like

```plaintext
[products ids="12,34,56"]
```

you can control **how many products per row** (columns), how many total (limit), and spacing through shortcode attributes and CSS.

---

### ⚙️ **1️⃣ Control layout via shortcode parameters**

Add these optional settings:

```plaintext
[products ids="12,34,56" columns="3" limit="6"]
```

* `columns="3"` → number of products per row
* `limit="6"` → how many total products to show

---

### ⚙️ **2️⃣ Adjust thumbnail sizes (global setting)**

WooCommerce controls thumbnail size from the Customizer:

1. Go to **WordPress Dashboard → Appearance → Customize**
2. Navigate to **WooCommerce → Product Images**
3. You can adjust:

   * **Main image width**
   * **Thumbnail width**
   * **Thumbnail cropping (1:1, custom, uncropped)**
4. Click **Publish**

This affects **all product grids**, including shortcodes.

---

### ⚙️ **3️⃣ Add custom CSS for finer control**

If you only want to resize products **on a specific page**, you can add custom CSS.

Example:

```css
/* Resize WooCommerce products on a custom Elementor page */
.custom-products .woocommerce ul.products li.product {
  width: 30%;          /* controls product card width */
  margin: 1% auto;
}

.custom-products .woocommerce ul.products li.product img {
  height: 250px;       /* set product image height */
  object-fit: cover;   /* crop image neatly */
}
```

Then wrap your shortcode inside a div with class `custom-products`:

```html
<div class="custom-products">
  [products ids="12,34,56" columns="3"]
</div>
```

In Elementor:

* Add a **Shortcode widget**
* Open **Advanced → CSS Classes**
* Add `custom-products`
* Paste the CSS into your theme or Elementor’s **Custom CSS** (Elementor Pro) section.

---

## 🟨 **If You’re Using Elementor’s WooCommerce Widgets (Pro version)**

Elementor Pro gives you direct visual controls:

1. Add a **Products** widget.
2. Under the **Style** tab → you can adjust:

   * **Image width & height**
   * **Spacing between items**
   * **Number of columns**
   * **Typography and button size**

No shortcode or CSS required — all visual.

---

## **Pro Tip**

If you only use shortcodes (no Elementor Pro), your best control options are:

* Use shortcode parameters (`columns`, `limit`)
* Adjust image sizes in **Customizer → WooCommerce → Product Images**
* Add small custom CSS for extra polish.

---
