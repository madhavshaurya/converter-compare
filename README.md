# ID Converter, Reverter & Comparator

A lightweight browser-based utility for converting, formatting, and comparing ID lists.

Perfect for developers, ERP users, database administrators, operations teams, and anyone who frequently works with large lists of IDs, document numbers, SKUs, order IDs, or invoice references.

## Features

### Convert List to Comma-Separated Format

Transform:

```text
ID001
ID002
ID003
```

into:

```text
ID001, ID002, ID003
```

---

### Convert Comma-Separated Values to List

Transform:

```text
ID001, ID002, ID003
```

into:

```text
ID001
ID002
ID003
```

---

### Wrap Values in Quotes

Useful for SQL queries and scripting.

#### Single Quotes

```sql
'ID001', 'ID002', 'ID003'
```

#### Double Quotes

```json
"ID001", "ID002", "ID003"
```

---

### Compare Two Lists

Compare:

* Master List
* Processed List

and instantly identify:

#### Missing Values

Items present in List A but missing from List B.

#### Extra Values

Items present in List B but not in List A.

---

### Copy to Clipboard

One-click copy support for:

* Input data
* Generated output

---

## Use Cases

### SQL IN Queries

```sql
SELECT *
FROM tabSales Order
WHERE name IN (
'SO-0001',
'SO-0002',
'SO-0003'
);
```

### ERPNext / Frappe

* Compare Purchase Orders
* Compare Sales Orders
* Compare Delivery Notes
* Compare SKU Lists
* Validate Data Migration

### Inventory Reconciliation

* Missing Articles
* Missing SKUs
* Warehouse Validation

### Data Cleaning

* Normalize ID Lists
* Remove unnecessary formatting
* Convert between list formats

---

## Tech Stack

* HTML5
* CSS3
* Vanilla JavaScript

No external dependencies.

No backend required.

Runs entirely in the browser.

---

## Local Development

Clone the repository:

```bash
git clone https://github.com/yourusername/id-converter.git
```

Navigate to the project:

```bash
cd id-converter
```

Open:

```bash
converterV3.html
```

in your browser.

---

## Deploy on Vercel

### Option 1: Via GitHub

1. Push the project to GitHub.
2. Login to Vercel.
3. Click **New Project**.
4. Import the GitHub repository.
5. Deploy.

No build settings are required.

### Option 2: Using Vercel CLI

Install Vercel CLI:

```bash
npm install -g vercel
```

Deploy:

```bash
vercel
```

For production:

```bash
vercel --prod
```

---

## Project Structure

```text
.
├── converterV3.html
└── README.md
```

---

## Future Enhancements

* Export results as CSV
* Export results as TXT
* Dark Mode
* Duplicate Detection
* Case-insensitive Comparison
* Ignore Whitespace Mode
* Copy Missing IDs
* Copy Extra IDs
* Drag & Drop File Upload

---

## License

MIT License

Feel free to use, modify, and distribute.
