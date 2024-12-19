# JSON to Table Viewer

This tool allows you to easily view JSON arrays in a table format directly in your browser. It includes functionality for sorting columns, hiding and restoring columns, dragging and dropping columns to reorder them, resizing columns, and filtering rows based on text input.

## Features

- **Paste JSON from Clipboard**: Click the **Paste JSON** button to read JSON data from your clipboard. The JSON should be an array of objects, where each object’s keys represent column names.
  
- **Table Generation**: Once the JSON is pasted, the tool automatically generates a sortable, filterable, and customizable table from the data.

- **Sorting Columns**: Click a column header to sort the table by that column. Each click toggles ascending/descending order.

- **Hiding Columns**: Right-click on a column header to hide that column. Hidden columns can be restored using the dropdown menu above the table.

- **Reordering Columns**: Drag and drop column headers (using the hamburger icon) to reorder columns. The new order is saved to `localStorage`, so the column order is preserved on page reload.

- **Resizing Columns**: Hover over the right edge of a column header until the resize indicator appears, then click and drag to adjust column width. Resized widths are stored in `localStorage`, so they remain consistent across sessions.

- **Filtering Rows**: Type in the filter input box above the table to quickly filter visible rows based on text content.

- **Local Persistence**: The tool uses `localStorage` to remember:
  - Hidden columns
  - Column order
  - Column widths

  This means your table configuration persists across page reloads.

## Getting Started

1. Clone or download this repository.
2. Open the `index.html` file in your browser.
3. Click the **Paste JSON** button. Ensure you have valid JSON (array of objects) copied to your clipboard.
4. Once the table is generated, you can:
   - Sort columns by clicking on headers.
   - Right-click headers to hide/show columns.
   - Drag to reorder columns.
   - Hover on the right side of a header to resize columns.
   - Use the filter input to narrow down rows.

## JSON Format Example

Your JSON should look like this (copied to your clipboard):

```json
[
  { "Name": "Alice", "Age": 30, "Role": "Developer" },
  { "Name": "Bob", "Age": 25, "Role": "Designer" },
  { "Name": "Charlie", "Age": 35, "Role": "Manager" }
]
