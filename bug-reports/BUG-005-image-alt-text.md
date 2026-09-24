#  BUG-005 — Generic or Missing Alternative Text for Images

![Severity](https://img.shields.io/badge/Severity-Medium-orange)
![Priority](https://img.shields.io/badge/Priority-Medium-yellow)
![Type](https://img.shields.io/badge/Type-Accessibility-blue)

---

##  Location

**Website:**  
https://www.shopup.org/

**Area:**  
Images across the public website

---

##  Steps to Reproduce

1. Open https://www.shopup.org/
2. Open Firefox Developer Tools.
3. Go to the **Console** tab.
4. Run the following JavaScript:

```javascript
[...document.images]
  .map((img, index) => ({
    index,
    alt: img.getAttribute('alt'),
    src: img.currentSrc || img.src
  }))
  .filter(x => !x.alt || x.alt.trim().toLowerCase() === 'image');
```
5. Review the returned images.
6. Verify the corresponding images on the page.

## Actual Result

Some images may have:

- No alt attribute, or
- A generic value such as image

This does not provide meaningful information about the image content.

## Expected Result

Images that convey meaningful information should have descriptive alternative text.
For example: 

```HTML
<img src="..." alt="ShopUp customer testimonial">
```

Decorative images should be appropriately marked as decorative rather than given meaningless alternative text.

## Impact

- Reduces accessibility for users who rely on screen readers.
- Makes image content difficult to understand when images cannot be viewed.
- Generic alternative text such as image provides little contextual information.
- May affect the overall accessibility quality of the website.

## 📸 Evidence

### Image Alternative Text

![BUG-005 — Image Alternative Text](https://github.com/user-attachments/assets/81048be7-518d-4c83-ad47-32d37210208f)

*Screenshot showing the image element and its generic or missing alternative text.*
