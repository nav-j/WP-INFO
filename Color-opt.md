# **FIX: Variation Swatches for WooCommerce Not Showing Colors**

---

## **Step 1: Check That Product Type = Variable Product**

First, make sure your product is not “Simple Product.”

1. Go to **Products → All Products**
2. Edit your product
3. In the **Product data** dropdown, ensure it’s set to
   👉 **Variable product**

If it says “Simple product,” color variations will never show.

---

## **Step 2: Create a *Global Attribute* for Color (Not Custom)**

This is the step most people miss.
The plugin only converts **global attributes** (made in WooCommerce → Attributes), not “custom” ones made inside a single product.

Here’s how 👇

### ➤ Create Global Attribute

1. Go to **Dashboard → Products → Attributes**
2. In **Name**, type `Color`
3. Choose **Type: Color** (you’ll see options like “Select,” “Color,” “Image”)
4. Click **Add attribute**

---

### ➤ Add Color Terms

After you create “Color,” it will appear in the right column.
Now add individual color values:

1. Click **Configure terms** next to “Color”
2. Add colors like:

   * Name: Red → Color: 🔴 (pick red color)
   * Name: Blue → Color: 🔵
   * Name: Black → Color: ⚫
   * Name: White → Color: ⚪
3. Click **Add new Color** each time.

Now WooCommerce knows what each color looks like.

---

## **Step 3: Assign the Global Color Attribute to the Product**

1. Edit your variable product again.
2. Go to the **Attributes** tab in the Product data box.
3. From the dropdown, select your **global “Color”** attribute (not custom).
4. Click **Add**.
5. Check ✅ “Used for variations.”
6. Select the colors (Red, Blue, etc.) for this product.
7. Click **Save attributes**.

---

## **Step 4: Create Variations from Colors**

1. Go to the **Variations** tab.
2. From the dropdown, choose:
   👉 “Create variations from all attributes” → Click **Go**
3. WooCommerce will generate one variation per color.
4. Set price and image for each variation.
5. Click **Save changes.**

---

## **Step 5: Clear Cache and Check Frontend**

Now visit the product page:
✅ You should see **colored circles (swatches)** instead of dropdowns.

If not visible yet:

* Clear your browser cache
* Clear your WordPress or theme cache (if you use caching plugins)
* Check the **plugin settings** (next step)

---

## **Step 6: Plugin Settings (Important)**

Go to
**Dashboard → WooCommerce → Swatches**

Make sure the following are enabled:

* ✅ “Enable Variation Swatches on Shop/Archive Pages” (optional but useful)
* ✅ “Show Swatches in Product Page”
* ✅ “Enable Tooltips” (optional)
* ✅ “Use Variation Image for Swatch” (if you want swatch color to change when selecting variation)

Click **Save Changes**

---

## **Common Mistakes**

| Problem                | Cause                                             | Fix                             |
| ---------------------- | ------------------------------------------------- | ------------------------------- |
| Still showing dropdown | Used “Custom product attribute” instead of global | Recreate attribute globally     |
| Swatches not colored   | Didn’t set a color value for each term            | Configure terms → Set color     |
| Images not changing    | Didn’t assign unique image to each variation      | Edit each variation → Add image |
| Plugin not applying    | Caching issue                                     | Clear cache / refresh page      |

---

## 🎉 **Result**

Once all steps are correct, your product page will show:

* Small **color circles** instead of dropdowns
* Clicking a color changes product image instantly

Works in both **default WooCommerce** and **Elementor product templates**.

---
