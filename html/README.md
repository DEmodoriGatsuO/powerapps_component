# HTML Elements for Power Apps

This repository contains examples of HTML elements designed for use within Power Apps. Each element is created with inline styles and avoids the use of double quotes to ensure compatibility with Power Apps.

## Files

### VerticalTable.html

This file contains an example of a vertically oriented table. Each row represents a different set of data, and the columns are headers.

**Code:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vertical Table</title>
</head>
<body>
    <h2>Vertical Table</h2>
    <table border=1 style='width: 100%; border-collapse: collapse;'>
        <thead>
            <tr>
                <th style='padding: 8px; background-color: #f2f2f2; text-align: left;'>Header 1</th>
                <th style='padding: 8px; background-color: #f2f2f2; text-align: left;'>Header 2</th>
                <th style='padding: 8px; background-color: #f2f2f2; text-align: left;'>Header 3</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td style='padding: 8px;'>Row 1, Cell 1</td>
                <td style='padding: 8px;'>Row 1, Cell 2</td>
                <td style='padding: 8px;'>Row 1, Cell 3</td>
            </tr>
            <tr>
                <td style='padding: 8px;'>Row 2, Cell 1</td>
                <td style='padding: 8px;'>Row 2, Cell 2</td>
                <td style='padding: 8px;'>Row 2, Cell 3</td>
            </tr>
            <tr>
                <td style='padding: 8px;'>Row 3, Cell 1</td>
                <td style='padding: 8px;'>Row 3, Cell 2</td>
                <td style='padding: 8px;'>Row 3, Cell 3</td>
            </tr>
        </tbody>
    </table>
</body>
</html>
```

### HorizontalTable.html

This file contains an example of a horizontally oriented table. Each column represents a different set of data, and the rows are headers.

**Code:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Horizontal Table</title>
</head>
<body>
    <h2>Horizontal Table</h2>
    <table border=1 style='width: 100%; border-collapse: collapse;'>
        <thead>
            <tr>
                <th style='padding: 8px; background-color: #f2f2f2; text-align: left;'>Header 1</th>
                <td style='padding: 8px;'>Row 1, Cell 1</td>
                <td style='padding: 8px;'>Row 2, Cell 1</td>
                <td style='padding: 8px;'>Row 3, Cell 1</td>
            </tr>
        </thead>
        <tbody>
            <tr>
                <th style='padding: 8px; background-color: #f2f2f2; text-align: left;'>Header 2</th>
                <td style='padding: 8px;'>Row 1, Cell 2</td>
                <td style='padding: 8px;'>Row 2, Cell 2</td>
                <td style='padding: 8px;'>Row 3, Cell 2</td>
            </tr>
            <tr>
                <th style='padding: 8px; background-color: #f2f2f2; text-align: left;'>Header 3</th>
                <td style='padding: 8px;'>Row 1, Cell 3</td>
                <td style='padding: 8px;'>Row 2, Cell 3</td>
                <td style='padding: 8px;'>Row 3, Cell 3</td>
            </tr>
        </tbody>
    </table>
</body>
</html>
```

### CombinedElements.html

This file contains examples of various HTML elements including tables, an unordered list, a simple bar chart, and an image. The elements are arranged both vertically and horizontally.

**Code:**
```html
<body>
    <!-- Vertical Table -->
    <h2>Vertical Table</h2>
    <table border=1 style='width: 100%; border-collapse: collapse;'>
        <thead>
            <tr>
                <th style='padding: 8px; background-color: #f2f2f2; text-align: left;'>Header 1</th>
                <th style='padding: 8px; background-color: #f2f2f2; text-align: left;'>Header 2</th>
                <th style='padding: 8px; background-color: #f2f2f2; text-align: left;'>Header 3</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td style='padding: 8px;'>Row 1, Cell 1</td>
                <td style='padding: 8px;'>Row 1, Cell 2</td>
                <td style='padding: 8px;'>Row 1, Cell 3</td>
            </tr>
            <tr>
                <td style='padding: 8px;'>Row 2, Cell 1</td>
                <td style='padding: 8px;'>Row 2, Cell 2</td>
                <td style='padding: 8px;'>Row 2, Cell 3</td>
            </tr>
            <tr>
                <td style='padding: 8px;'>Row 3, Cell 1</td>
                <td style='padding: 8px;'>Row 3, Cell 2</td>
                <td style='padding: 8px;'>Row 3, Cell 3</td>
            </tr>
        </tbody>
    </table>

    <!-- Horizontal Table -->
    <h2>Horizontal Table</h2>
    <table border=1 style='width: 100%; border-collapse: collapse;'>
        <thead>
            <tr>
                <th style='padding: 8px; background-color: #f2f2f2; text-align: left;'>Header 1</th>
                <td style='padding: 8px;'>Row 1, Cell 1</td>
                <td style='padding: 8px;'>Row 2, Cell 1</td>
                <td style='padding: 8px;'>Row 3, Cell 1</td>
            </tr>
        </thead>
        <tbody>
            <tr>
                <th style='padding: 8px; background-color: #f2f2f2; text-align: left;'>Header 2</th>
                <td style='padding: 8px;'>Row 1, Cell 2</td>
                <td style='padding: 8px;'>Row 2, Cell 2</td>
                <td style='padding: 8px;'>Row 3, Cell 2</td>
            </tr>
            <tr>
                <th style='padding: 8px; background-color: #f2f2f2; text-align: left;'>Header 3</th>
                <td style='padding: 8px;'>Row 1, Cell 3</td>
                <td style='padding: 8px;'>Row 2, Cell 3</td>
                <td style='padding: 8px;'>Row 3, Cell 3</td>
            </tr>
        </tbody>
    </table>

    <!-- Flexbox Container -->
    <h2>Horizontal Layout</h2>
    <div style='display: flex; justify-content: space-around; align-items: flex-start;'>
        <!-- Unordered List -->
        <div style='margin: 10px;'>
            <h3>Unordered List</h3>
            <ul>
                <li>Item 1</li>
                <li>Item 2</li>
                <li>Item 3</li>
            </ul>
        </div>

        <!-- Simple Bar Chart -->
        <div style='margin: 10px;'>
            <h3>Simple Bar Chart</h3>
            <svg width='150' height='200'>
                <rect x='10' y='10' width='50' height='150' style='fill:blue;'></rect>
                <rect x='70' y='40' width='50' height='120' style='fill:green;'></rect>
                <rect x='130' y='70' width='50' height='90' style='fill:red;'></rect>
            </svg>
        </div>

        <!-- Image -->
        <div style='margin: 10px;'>
            <h3>Image</h3>
            <img src='https://via.placeholder.com/150' alt='Sample Image' style='width:150px;height:150px;'>
        </div>
    </div>
</body>
```

## Usage

To use these HTML files in Power Apps, copy the contents of the desired file and paste it into an HTML Text control within your Power Apps application.