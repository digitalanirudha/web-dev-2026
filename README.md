
# HTML Single Page Website with No CSS

Build a html web page using html tags. Added some properties to html tags as inline css to make it more readable.

Website link : https://codeparser.cloud/

GitHub Path : https://github.com/digitalanirudha/web-dev-2026/blob/main/html/html-webpage

GitHub Folder : https://github.com/digitalanirudha/web-dev-2026/tree/main/html


# Learning Summary

## Overview
This portfolio page is created using **ONLY HTML** - no CSS is used. We make it attractive using HTML attributes and table-based layout.

---

## 1. Basic HTML Structure

### Document Setup
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anirudha D.- Portfolio</title>
</head>
<body>
```

**What it does:**
- `<!DOCTYPE html>` - Tells browser this is HTML5
- `<html lang="en">` - Root element, language set to English
- `<head>` - Contains meta information (not visible on page)
- `<meta charset="UTF-8">` - Sets character encoding for special characters
- `<meta name="viewport">` - Makes page responsive on mobile devices
- `<title>` - Shows in browser tab
- `<body>` - Contains all visible content

---

## 2. Body Tag Attributes

```html
<body bgcolor="#E8E8E8" text="#333333">
```

**Attributes used:**
- `bgcolor="#E8E8E8"` - Sets light gray background color for entire page
- `text="#333333"` - Sets dark gray color for all text

**Color format:** `#` followed by 6 characters (hex color code)

---

## 3. Table Layout Structure

### Main Container Table
```html
<table width="80%" align="center" cellpadding="20" bgcolor="#F5F5F5" border="0">
```

**Attributes explained:**
- `width="80%"` - Table takes 80% of screen width
- `align="center"` - Centers the table on page
- `cellpadding="20"` - Adds 20 pixels of space inside cells
- `bgcolor="#F5F5F5"` - Light background color for the container
- `border="0"` - No visible border (0 = invisible)

### Why use tables?
Tables create a structured layout without CSS. Each section is placed in table rows and cells.

---

## 4. Font Tag - Styling Text

```html
<font size="7" color="white" face="Calibri, sans-serif">
    <b>Anirudha D.</b>
</font>
```

**Font attributes:**
- `size` - Text size (1-7, where 7 is largest)
- `color` - Text color (can use names like "white" or hex codes like "#4A90E2")
- `face` - Font family (Calibri, Calibri, etc.)

**Common sizes used in this page:**
- Size 7 - Main heading (name)
- Size 5 - Section headings
- Size 4 - Subheadings
- Size 3 - Regular text
- Size 2 - Footer text

---

## 5. Text Formatting Tags

```html
<b>Bold Text</b>           - Makes text bold
<i>Italic Text</i>         - Makes text italic
<br>                       - Line break (new line)
<hr color="#CCCCCC">       - Horizontal line with color
```

**Usage in page:**
- `<b>` - Used for important words, headings, labels
- `<i>` - Used for subtitle in header
- `<br>` - Creates spacing between elements
- `<hr>` - Separates projects

---

## 6. Lists

```html
<ul>
    <li><b>HTML5 & CSS3</b></li>
    <li><b>JavaScript</b></li>
</ul>
```

**List tags:**
- `<ul>` - Unordered list (bullet points)
- `<li>` - List item

**Where used:**
- Skills section
- Project details (technologies & timeline)

---

## 7. Table Sections

### Section Header Pattern
```html
<table width="100%" cellpadding="15" bgcolor="#FFFFFF" border="1" bordercolor="#CCCCCC">
    <tr bgcolor="#5A9FD4">
        <td>
            <font size="5" color="white" face="Calibri, sans-serif">
                <b>About Me</b>
            </font>
        </td>
    </tr>
    <tr>
        <td>
            <!-- Content here -->
        </td>
    </tr>
</table>
```

**Pattern breakdown:**
- Outer table with white background and gray border
- First row (`<tr>`) has blue background with white heading
- Second row contains the actual content

---

## 8. Data Tables (Experience & Education)

```html
<tr bgcolor="#7AB8E8" align="center">
    <td width="35%">
        <font size="3" color="white" face="Calibri, sans-serif">
            <b>Position</b>
        </font>
    </td>
</tr>
```

**Table attributes:**
- `<tr>` - Table row
- `<td>` - Table data cell
- `bgcolor` - Background color for row/cell
- `align="center"` - Centers content
- `width="35%"` - Sets column width
- `colspan="3"` - Makes cell span across 3 columns

**Alternating row colors:**
- `bgcolor="#F9F9F9"` - Light gray
- `bgcolor="#FFFFFF"` - White
Creates a striped effect for better readability

---

## 9. Color Scheme Used

| Color Code | Color Name | Usage |
|------------|------------|-------|
| #4A90E2 | Blue | Main header, section headings |
| #5A9FD4 | Medium Blue | Section header backgrounds |
| #7AB8E8 | Light Blue | Table headers |
| #FFFFFF | White | Content backgrounds |
| #F9F9F9 | Very Light Gray | Alternating table rows |
| #E8E8E8 | Light Gray | Page background |
| #CCCCCC | Gray | Borders |
| #333333 | Dark Gray | Text color |

---

## 10. Special Characters

```html
&copy;  - © (copyright symbol)
```

**Usage:**
- Footer: `&copy; 2026 Anirudha D.`

---

## 11. Complete Section Example

### Contact Section Breakdown
```html
<!-- Contact Section -->
<table width="100%" cellpadding="15" bgcolor="#FFFFFF" border="1" bordercolor="#CCCCCC">
    <!-- Blue header row -->
    <tr bgcolor="#5A9FD4">
        <td>
            <font size="5" color="white" face="Calibri, sans-serif">
                <b>Contact</b>
            </font>
        </td>
    </tr>
    <!-- Content row -->
    <tr>
        <td>
            <font size="3" face="Arial, sans-serif">
                <b>Email:</b> <font color="#4A90E2">anirudhad@example.com</font>
            </font>
            <br><br>
            <font size="3" face="Arial, sans-serif">
                <b>Phone:</b> <font color="#4A90E2">+1 (555) 123-4567</font>
            </font>
            <br><br>
            <font size="3" face="Arial, sans-serif">
                <b>Location:</b> <font color="#4A90E2">Madhya Pradesh, India</font>
            </font>
        </td>
    </tr>
</table>
```

---

## 12. Key Learning Points

### ✅ What you Should Understand:

1. **HTML Attributes** - Add properties to elements (bgcolor, width, align, etc.)
2. **Tables for Layout** - Use nested tables to create page structure
3. **Font Tag** - Control text appearance (size, color, font)
4. **Color Codes** - Hex codes (#RRGGBB) for custom colors
5. **Nesting** - Elements inside elements (tables in tables, fonts in fonts)
6. **Structure** - Organize content in logical sections

### ✅ HTML Tags Used in This Page:

- **Structure:** `<html>`, `<head>`, `<body>`, `<table>`, `<tr>`, `<td>`
- **Text:** `<font>`, `<b>`, `<i>`, `<br>`, `<hr>`
- **Lists:** `<ul>`, `<li>`
- **Meta:** `<meta>`, `<title>`

### ✅ HTML Attributes Used:

- **Layout:** `width`, `align`, `cellpadding`, `border`, `colspan`
- **Colors:** `bgcolor`, `color`, `bordercolor`
- **Text:** `size`, `face`

---

## 13. Why This Approach?

**Advantages:**
✓ No CSS needed - works in any browser
✓ Simple for beginners
✓ Shows how HTML attributes work
✓ Good for learning table structures

**Limitations:**
✗ Repetitive code (font tags everywhere)
✗ Hard to maintain for large sites
✗ Modern websites use CSS instead
✗ Not responsive on all devices

**Best Practice:** This is great for learning HTML, but in real projects, use CSS for styling!

---

## 14. Practice Exercises for Students

1. **Change Colors:** Try different color codes for backgrounds and text
2. **Add Section:** Create a "Hobbies" or "Certifications" section
3. **Modify Layout:** Change table widths and padding
4. **Add Content:** Add more projects or experience entries
5. **Experiment:** Try different font sizes and faces

---

## 15. Common Mistakes to Avoid

❌ Forgetting closing tags (`</table>`, `</font>`, `</td>`)
❌ Mismatched colors (dark text on dark background)
❌ Not using `colspan` when headers span multiple columns
❌ Forgetting `<tr>` and `<td>` tags in tables
❌ Using wrong color codes (must start with #)

---

## Summary

This portfolio page demonstrates how to create an attractive website using **only HTML attributes** - no CSS required! It uses tables for layout, font tags for styling, and various attributes for colors and spacing. While modern web development uses CSS for styling, understanding these HTML fundamentals is essential for every web developer.

**Key takeaway:** HTML can do more than just structure - it can also style content using attributes!
