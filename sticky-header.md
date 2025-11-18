Here are **three simple ways** to make a **sticky header in WordPress** (no coding, low-coding, and full-coding options).
Choose the one that fits your setup (Theme, Elementor, or custom code).

---

# ✅ **Method 1: Using WordPress Theme Settings (Easiest)**

Most themes like **Astra, GeneratePress, OceanWP, Neve, Kadence** already have a sticky header option.

### **Steps**

1. Go to **Appearance → Customize**
2. Open **Header**
3. Look for **Sticky Header / Fixed Header / Sticky Navigation**
4. Turn ON the feature
5. Publish

If your theme supports it → *No code needed*.

---

# ✅ **Method 2: Using Elementor (Very Common)**

### **Steps (Elementor Pro required for Motion Effects)**

1. Edit your **Header template** from
   **Templates → Theme Builder → Header**
2. Select the **Section** containing the header.
3. Go to **Advanced → Motion Effects**
4. Find **Sticky**
5. Choose:
   ✔ *Top*
   ✔ *On scroll*
6. Turn on **Sticky On: Desktop / Tablet / Mobile**
7. Update

Your header will now stick at the top when scrolling.

---

# ✅ **Method 3: Using Simple CSS (Works with Any Theme)**

If your theme does NOT support a sticky header, you can add CSS.

### **Steps**

1. Go to **Appearance → Customize → Additional CSS**
2. Add this CSS:

```css
/* Make header sticky */
header {
    position: sticky;
    top: 0;
    z-index: 9999;
    background: white;
}
```

If your header uses a different selector, replace `header` with:

* `.site-header`
* `.main-header`
* `.navbar`
* `.header-area`
  (whichever your theme uses)

---

# 🔧 **If Your Header Height Changes on Scroll (Shrinking Header)**

Add this:

```css
header {
    position: sticky;
    top: 0;
    z-index: 9999;
    transition: all 0.3s;
}

header.sticky-header {
    padding: 5px 0;
}
```

And add JavaScript in **Appearance → Theme File Editor → footer.php** before `</body>`:

```html
<script>
window.addEventListener("scroll", function () {
    const header = document.querySelector("header");
    header.classList.toggle("sticky-header", window.scrollY > 50);
});
</script>
```
