
# HTML Single Page Website with No CSS

Build a html web page using html tags. Added some properties to html tags as inline css to make it more readable.

Website link : https://codeparser.cloud/

GitHub Path : https://github.com/digitalanirudha/web-dev-2026/blob/main/html/html-webpage

GitHub Folder : https://github.com/digitalanirudha/web-dev-2026/tree/main/html


# Learning Summary
## Technical Evaluation

## Overview
This HTML portfolio page demonstrates table-based layout using **ONLY HTML attributes** for styling - no external CSS files. It showcases inline styling techniques and nested table structures to create a professional multi-section portfolio.

---

## 1. Document Structure

### HTML5 Declaration
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anirudha D.- Portfolio</title>
</head>
<body bgcolor="#E8E8E8" text="#333333">
```

**Technical breakdown:**
- `<!DOCTYPE html>` - HTML5 standard document type declaration
- `<html lang="en">` - Root element with English language attribute
- `<meta charset="UTF-8">` - Character encoding for international characters support
- `<meta name="viewport">` - Responsive viewport configuration for mobile devices
- `<title>` - Browser tab title and SEO element
- `bgcolor="#E8E8E8"` - Deprecated body background color attribute
- `text="#333333"` - Deprecated default text color attribute

---

## 2. Main Container Architecture

### Master Table Structure
```html
<table width="80%" align="center" cellpadding="20" bgcolor="#F5F5F5" border="0">
    <tr>
        <td>
            <!-- All content nested here -->
        </td>
    </tr>
</table>
```

**Attributes explained:**
- `width="80%"` - Responsive width, takes 80% of browser window
- `align="center"` - Centers table horizontally on page
- `cellpadding="20"` - Internal padding of 20 pixels inside cells
- `bgcolor="#F5F5F5"` - Off-white background color
- `border="0"` - Removes table border (invisible borders)

**Purpose:** Creates centered container with whitespace margins (10% on each side)

---

## 3. Header Section Implementation

### Header Table
```html
<table width="100%" cellpadding="15" bgcolor="#708090" border="0">
    <tr>
        <td align="center">
            <font size="7" color="white" face="Calibri, sans-serif">
                <b>Anirudha D.</b>
            </font>
            <br>
            <font size="4" color="#E0E0E0" face="Calibri, sans-serif">
                <i>Full Stack Developer | REST API | Tech Enthusiast</i>
            </font>
        </td>
    </tr>
</table>
```

**Technical details:**
- `bgcolor="#708090"` - Slate gray background (professional color)
- `size="7"` - Maximum font size for primary heading
- `size="4"` - Medium size for subtitle
- `color="white"` - High contrast on dark background
- `color="#E0E0E0"` - Slightly dimmed white for secondary text
- `face="Calibri, sans-serif"` - Font family with fallback
- `<b>` - Bold tag for name emphasis
- `<i>` - Italic tag for tagline styling

---

## 4. Section Pattern Structure

### Standard Section Template
```html
<table width="100%" cellpadding="15" bgcolor="#FFFFFF" border="1" bordercolor="#CCCCCC">
    <!-- Section Header Row -->
    <tr bgcolor="#36454F">
        <td>
            <font size="5" color="white" face="Calibri, sans-serif">
                <b>Section Title</b>
            </font>
        </td>
    </tr>
    <!-- Content Row -->
    <tr>
        <td>
            <font size="3" face="Calibri, sans-serif">
                Content goes here
            </font>
        </td>
    </tr>
</table>
```

**Pattern breakdown:**
- Outer table: `border="1"` with `bordercolor="#CCCCCC"` creates gray borders
- Header row: `bgcolor="#36454F"` (charcoal gray) with white text
- Content row: White background with structured content
- Consistent `cellpadding="15"` for uniform spacing

**Used in sections:** About Me, Skills, Projects, Contact

---

## 5. Font Tag Implementation

### Typography Control
```html
<font size="3" color="#4A90E2" face="Calibri, sans-serif">
    Text content
</font>
```

**Font attributes:**
- `size` - Range 1-7 (where 7 is largest, 3 is default body text)
- `color` - Hex codes (#RRGGBB) or named colors (white, black, etc.)
- `face` - Font family with comma-separated fallbacks

**Size hierarchy in this portfolio:**
| Size | Usage | Example |
|------|-------|---------|
| 7 | Main heading | Name in header |
| 5 | Section headings | About Me, Skills, Experience |
| 4 | Subheadings | Tagline, project titles |
| 3 | Body text | Paragraphs, descriptions |
| 2 | Footer text | Copyright notice |

---

## 6. Data Table Structure

### Experience & Education Tables
```html
<table width="100%" cellpadding="15" bgcolor="#FFFFFF" border="1" bordercolor="#CCCCCC">
    <tr bgcolor="#36454F">
        <td colspan="3">
            <font size="5" color="white" face="Calibri, sans-serif">
                <b>Experience</b>
            </font>
        </td>
    </tr>
    <tr bgcolor="#71797E" align="center">
        <td width="35%">
            <font size="3" color="white" face="Calibri, sans-serif">
                <b>Position</b>
            </font>
        </td>
        <td width="40%">
            <font size="3" color="white" face="Calibri, sans-serif">
                <b>Company</b>
            </font>
        </td>
        <td width="25%">
            <font size="3" color="white" face="Calibri, sans-serif">
                <b>Duration</b>
            </font>
        </td>
    </tr>
    <tr bgcolor="#F9F9F9">
        <td><!-- Position --></td>
        <td><!-- Company --></td>
        <td><!-- Duration --></td>
    </tr>
</table>
```

**Advanced table features:**
- `colspan="3"` - Section header spans across all 3 columns
- `width="35%"` / `width="40%"` / `width="25%"` - Fixed column proportions (total 100%)
- `align="center"` - Centers column headers
- Alternating `bgcolor="#F9F9F9"` and `bgcolor="#FFFFFF"` - Zebra striping for readability

---

## 7. List Implementation

### Unordered List in Skills Section
```html
<font size="3" face="Calibri, sans-serif">
    <ul>
        <li><b>HTML5 & CSS3</b></li>
        <li><b>JavaScript</b></li>
        <li><b>React & Vue.js</b></li>
        <li><b>Node.js & Express</b></li>
        <li><b>MongoDB & MySQL</b></li>
        <li><b>Git & GitHub</b></li>
    </ul>
</font>
```

**List elements:**
- `<ul>` - Unordered list (bullet points)
- `<li>` - List item (each skill)
- `<b>` - Bold formatting for emphasis
- Wrapped in `<font>` tag for consistent styling

---

## 8. Projects Section Pattern

### Multi-Content Section
```html
<tr>
    <td>
        <font size="4" color="#4A90E2" face="Calibri, sans-serif">
            <b>Project 1: E-Commerce Website</b>
        </font>
        <br><br>
        <font size="3" face="Georgia, serif">
            Built a fully functional e-commerce platform...
        </font>
        <ul>
            <li><font size="3" face="Calibri, sans-serif"><b>Technologies:</b> React, Node.js, MongoDB</font></li>
            <li><font size="3" face="Calibri, sans-serif"><b>Timeline:</b> 6 months</font></li>
        </ul>
        
        <hr color="#CCCCCC">
        
        <font size="4" color="#4A90E2" face="Calibri, sans-serif">
            <b>Project 2: Blog Platform</b>
        </font>
        <!-- More content -->
    </td>
</tr>
```

**Technical features:**
- `<br><br>` - Double line break for vertical spacing
- `face="Georgia, serif"` - Different font for descriptions (serif for readability)
- `<hr color="#CCCCCC">` - Horizontal rule separator between projects
- Nested lists within table cells
- Color-coded project titles (`color="#4A90E2"`)

---

## 9. Color Scheme Implementation

### Complete Color Palette
```
Header Backgrounds:
- #708090 (Slate Gray) - Main header
- #36454F (Charcoal) - Section headers
- #71797E (Gray) - Table column headers

Content Backgrounds:
- #FFFFFF (White) - Primary content areas
- #F9F9F9 (Off-white) - Alternating table rows
- #F5F5F5 (Light gray) - Main container
- #E8E8E8 (Lighter gray) - Page background

Accent Colors:
- #4A90E2 (Blue) - Links, highlights, project titles
- #E0E0E0 (Light gray) - Subtitle text

Borders:
- #CCCCCC (Medium gray) - Table borders, HR lines

Text:
- #333333 (Dark gray) - Default body text
- white - Headers and labels
```

---

## 10. Text Formatting Tags

### Inline Text Styling
```html
<b>Bold Text</b>              <!-- Bold emphasis -->
<i>Italic Text</i>            <!-- Italic styling -->
<br>                          <!-- Line break -->
<hr color="#CCCCCC">          <!-- Horizontal divider -->
```

**Usage patterns:**
- `<b>` - Labels (Email:, Phone:, Technologies:), important terms
- `<i>` - Tagline and subtle emphasis
- `<br>` - Spacing between contact details
- `<hr>` - Visual separator between projects

---

## 11. Special Characters

### HTML Entities
```html
&copy; 2026 Anirudha D. All rights reserved.
```

**Entity breakdown:**
- `&copy;` - Copyright symbol (©)
- Used in footer for professional copyright notice

---

## 12. Nested Table Architecture

### Nesting Structure
```
Main Container Table (80% width, centered)
└── Single TR
    └── Single TD
        ├── Header Table
        ├── <br>
        ├── About Me Table
        ├── <br>
        ├── Skills Table
        ├── <br>
        ├── Experience Table
        ├── <br>
        ├── Projects Table
        ├── <br>
        ├── Education Table
        ├── <br>
        ├── Contact Table
        ├── <br>
        └── Footer Table
```

**Purpose of nesting:**
- Main table provides container and centering
- Inner tables create individual sections
- `<br>` tags add vertical spacing between sections

---

## 13. Complete Section Analysis

### Contact Section Breakdown
```html
<!-- Contact Section -->
<table width="100%" cellpadding="15" bgcolor="#FFFFFF" border="1" bordercolor="#CCCCCC">
    <tr bgcolor="#36454F">
        <td>
            <font size="5" color="white" face="Calibri, sans-serif">
                <b>Contact</b>
            </font>
        </td>
    </tr>
    <tr>
        <td>
            <font size="3" face="Calibri, sans-serif">
                <b>Email:</b> <font color="#4A90E2">anirudhad@example.com</font>
            </font>
            <br><br>
            <font size="3" face="Calibri, sans-serif">
                <b>Phone:</b> <font color="#4A90E2">+91 9834 3434 37</font>
            </font>
            <br><br>
            <font size="3" face="Calibri, sans-serif">
                <b>Location:</b> <font color="#4A90E2">Madhya Pradesh, India</font>
            </font>
        </td>
    </tr>
</table>
```

**Technical implementation:**
- Nested `<font>` tags for different colors within same line
- `<b>` tags for labels (Email:, Phone:, Location:)
- Blue color (`#4A90E2`) for actual contact information
- `<br><br>` creates consistent spacing between contact items

---

## 14. HTML Tags Inventory

### Structural Tags
```
<html>        - Root document element
<head>        - Document metadata container
<body>        - Visible content container
<table>       - Table container
<tr>          - Table row
<td>          - Table data cell
```

### Text & Formatting Tags
```
<font>        - Text styling (size, color, face)
<b>           - Bold text
<i>           - Italic text
<br>          - Line break
<hr>          - Horizontal rule
```

### List Tags
```
<ul>          - Unordered list
<li>          - List item
```

### Meta Tags
```
<meta>        - Metadata (charset, viewport)
<title>       - Document title
```

---

## 15. HTML Attributes Reference

### Table Attributes
```
width="80%"           - Table/cell width (percentage or pixels)
align="center"        - Horizontal alignment
cellpadding="15"      - Internal cell padding
border="1"            - Border thickness
bordercolor="#CCC"    - Border color
bgcolor="#FFF"        - Background color
colspan="3"           - Column spanning
```

### Font Attributes
```
size="5"              - Font size (1-7)
color="#4A90E2"       - Text color
face="Calibri"        - Font family
```

### General Attributes
```
lang="en"             - Language attribute
charset="UTF-8"       - Character encoding
name="viewport"       - Viewport settings
```

---

## 16. Technical Observations

### Deprecated Elements Used
```
✗ <font> tag                - Deprecated in HTML5
✗ bgcolor attribute         - Use CSS background-color
✗ align attribute           - Use CSS text-align/float
✗ cellpadding attribute     - Use CSS padding
✗ border attribute          - Use CSS border
✗ size attribute (font)     - Use CSS font-size
✗ color attribute (font)    - Use CSS color
✗ face attribute (font)     - Use CSS font-family
```

**Modern equivalent:** All styling should be done with CSS

### Missing Modern Elements
```
✗ No semantic HTML5 tags    - <header>, <nav>, <section>, <article>, <footer>
✗ No CSS (inline or external)
✗ No JavaScript
✗ No accessibility features - ARIA labels, alt attributes
✗ No responsive design      - Fixed widths, no media queries
```

---

## 17. Code Quality Analysis
Why this is important to understand because HTML limitations needs to be understood and Why to use Modern CSS.

### Strengths
✓ Consistent indentation and formatting<br>
✓ Descriptive HTML comments for each section<br>
✓ Logical nesting structure<br>
✓ Proper closing of all tags<br>
✓ Coherent color scheme throughout<br>
✓ Alternating row colors for readability<br>
✓ Reusable section pattern<br>

### Weaknesses
✗ Repetitive font tag usage (DRY principle violated) <br>
✗ Inline attributes make maintenance difficult <br>
✗ No separation of concerns (structure + style mixed) <br>
✗ Not mobile-responsive <br>
✗ Accessibility issues (no semantic markup) <br>
✗ Uses deprecated HTML elements <br>
✗ Hard to scale for larger websites <br>

---

## 18. Browser Compatibility

**Compatibility:** Works in all browsers (Chrome, Firefox, Safari, Edge, IE)

**Reason:** Uses basic HTML elements that have been supported since HTML 3.2 (1997)

**Note:** While compatible, this approach is outdated for modern web development

---

## 19. Performance Considerations

### File Size
- Single HTML file: ~8-10 KB
- No external resources (CSS/JS files)
- Fast load time

### Rendering
- Simple DOM structure
- No CSS parsing required
- Minimal browser processing

---

## 20. Learning Outcomes

### Key Concepts Demonstrated
1. **Table-based layout** - Using tables for page structure
2. **Inline styling** - Applying styles via HTML attributes
3. **Nested structures** - Tables within tables
4. **Color theory** - Hex color codes and color contrast
5. **Typography** - Font sizing and font families
6. **Semantic grouping** - Organizing content in logical sections

### Modern Web Development Comparison
| Old Way (This Code) | Modern Way |
|---------------------|------------|
| `<font>` tags | CSS `font-size`, `color`, `font-family` |
| `bgcolor` attribute | CSS `background-color` |
| Table layout | CSS Flexbox/Grid |
| Inline attributes | External CSS files |
| No responsiveness | Media queries |
| Generic tags | Semantic HTML5 tags |

---

## Summary

This portfolio demonstrates **legacy HTML techniques** where all styling is achieved through HTML attributes without CSS. It uses a table-based layout with nested structures, font tags for typography, and inline color attributes. While functional and browser-compatible, this approach is deprecated in favor of modern CSS-based styling and semantic HTML5 structure.

**Educational Value:** Excellent for understanding HTML fundamentals and the evolution of web development, but should not be used in production environments.

**Key Takeaway:** Modern web development separates structure (HTML) from presentation (CSS) for maintainability, accessibility, and responsiveness.
