# **Show Color Swatches on Shop or Custom Product Pages**

---

## **Step 1: Enable Shop Page Swatches in Plugin Settings**

1. Go to
   **Dashboard → WooCommerce → Swatches**
2. Scroll to the section titled
   **“Archive / Shop Page Settings”**
3. Turn ON these options:

   * ✅ **Enable Variation Swatches on Archive/Shop Page**
   * ✅ **Show Tooltip on Archive/Shop Page** *(optional)*
   * ✅ **Use Variation Image for Swatch Preview** *(optional but nice effect)*
4. Click **Save Changes**

Now swatches should appear automatically on:

* `/shop` (default WooCommerce shop)
* Product category pages
* Any WooCommerce archive or loop (like `[products]` shortcode or Elementor’s “Products” widget)

---

## **Step 2: If Using Elementor Shortcode or Widget**

If your page uses:

```plaintext
[products]
```

or any `[products ...]` shortcode
👉 the swatches will automatically appear **if** Step 1 is done.

If you’re using **Elementor**:

1. Edit your custom page with Elementor
2. Add either:

   * **Shortcode widget** → paste `[products]` or `[products category="tshirts"]`, OR
   * **Products widget** (if you’re using Elementor Pro or WooCommerce widgets)
3. **Update page**
4. Refresh — you should now see swatches under each product card.

🧠 *Note:* Some themes may override WooCommerce templates — if you don’t see swatches, go to plugin settings → “Advanced” → enable **Force show on archive page**.

---

## **Step 3: Adjust Swatch Size & Style**

Still under
**WooCommerce → Swatches → Design / Style tab**

You can customize:

* 🔸 Swatch **shape:** Square / Rounded
* 🔸 Swatch **size:** e.g. 30px, 40px
* 🔸 Border & hover effects
* 🔸 Tooltip text color/background

Then click **Save Changes** again.

---

## **Step 4: Clear Cache**

If using any caching or optimization plugins (like WP Rocket, LiteSpeed, or SiteGround Optimizer), clear all caches — otherwise, you may still see the old view.

---

## ✅ **Result**

Now your **Shop page**, **custom Elementor product grids**, and **shortcode-based product listings** will all show:

* Beautiful color swatches
* Click-to-preview variation image
* No dropdowns anywhere 🎨

---
