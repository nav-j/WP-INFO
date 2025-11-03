# 🟩 STEP-BY-STEP: ADD PRODUCTS AVAILABLE IN DIFFERENT COLORS (WooCommerce)

---

## 🧩 **Step 1: Create or Edit a Product**

1. In your WordPress Dashboard → go to
   **Products → Add New** (or edit an existing one).

2. Enter your product details:

   * Product name (e.g., *T-shirt*)
   * Description
   * Featured image (default color or main image)

---

## 🎚️ **Step 2: Change Product Type to “Variable Product”**

Scroll down to the **Product data** box.
From the dropdown (top left of that box), select:

> **Variable product**

This allows you to add variations like **different colors** or **sizes**.

---

## 🎨 **Step 3: Create a Color Attribute**

1. In the same **Product data** box → Go to **Attributes** tab.
2. Click **Add** (choose “Custom product attribute”).
3. In **Name**, type `Color`.
4. In **Value(s)**, type your available colors — separated by `|`:

   ```
   Red | Blue | Black | White
   ```
5. Check ✅ **Used for variations**
6. Click **Save attributes**.

---

## 🧱 **Step 4: Create Variations for Each Color**

1. Go to the **Variations** tab.
2. From the dropdown → choose **“Create variations from all attributes”** → Click **Go**.
3. WooCommerce will auto-create one variation per color (Red, Blue, etc.).

Now you’ll see each color listed as its own variation.

---

## 🖼️ **Step 5: Add Details to Each Variation**

For each color:

1. Click the dropdown arrow beside it to expand.
2. Set:

   * **Regular price**
   * (Optional) **Sale price**
   * **Product image** (upload color-specific photo)
3. Repeat for all color variations.
4. Click **Save changes**.

---

## 🛒 **Step 6: Publish**

Click **Publish/Update** — your product now shows a **color dropdown** on the product page, letting buyers choose which color they want. 🎉

---

## 🟣 **How to Show It on Your Custom Page (Elementor or Shortcode)**

Once the product is published:

* If you’re using a **shortcode**, it’s automatically supported.
  Example:

  ```plaintext
  [products ids="34"]
  ```

  → The product box will appear with its variation options (color dropdown) on the product detail page.

✅ *Note:* WooCommerce only shows variation selectors on the **product detail page**, not in the grid/list view.
So on the grid (shop page or shortcode list), users will click the product → go to product page → then choose color.

---

## 🧠 **Bonus: Showing Color Options as Buttons or Swatches**

If you want **color buttons or image swatches instead of a dropdown**, you can use a free plugin:

### 🛠️ Recommended Plugins:

1. **Variation Swatches for WooCommerce** (by Emran Ahmed)
2. **Woo Variation Swatches** (by ThemeHigh)

After installing one:

* It replaces the default dropdown with **color circles or image swatches** automatically.
* Works perfectly with Elementor and shortcodes.

---

## ✅ **Summary**

| Step | Action                 | Result                            |
| ---- | ---------------------- | --------------------------------- |
| 1    | Create / Edit Product  | Add base info                     |
| 2    | Set “Variable Product” | Enable variations                 |
| 3    | Add “Color” Attribute  | Define colors                     |
| 4    | Create Variations      | Auto-create per color             |
| 5    | Set Prices & Images    | Customize each variation          |
| 6    | Publish                | Buyers can pick color             |
| 7    | (Optional) Use Plugin  | Show swatches instead of dropdown |

---
