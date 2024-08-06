# HTML Table Examples for Power Apps

This repository contains examples of HTML tables designed for use within Power Apps. Each table is created with inline styles and avoids the use of double quotes to ensure compatibility.

## Files

### VerticalTable.html

This file contains an example of a vertically oriented table. Each row represents a different set of data, and the columns are headers.

**Code:**
```html
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
```

### HorizontalTable.html

This file contains an example of a horizontally oriented table. Each column represents a different set of data, and the rows are headers.

**Code:**
```html
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
```

## Usage

To use these HTML files in Power Apps, copy the contents of the desired file and paste it into an HTML Text control within your Power Apps application.
```

### Save the Files

1. **VerticalTable.html**:
   Save the first HTML content into a file named `VerticalTable.html`.

2. **HorizontalTable.html**:
   Save the second HTML content into a file named `HorizontalTable.html`.

3. **README.md**:
   Save the README content into a file named `README.md`.

These files provide a comprehensive guide and examples for creating and using HTML tables within Power Apps