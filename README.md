# MoreDown

**Even more stripped‑down Markdown**

## 1. Overview
MoreDown is a minimal, GFM‑compatible subset designed for short‑form contexts (e.g. comment threads, tweets). Every MoreDown document is also valid GFM; any syntax not explicitly supported will be emitted as plain text.

## 2. Compatibility
- **Recommended file extension**: `.md`  
- **Base**: GitHub Flavored Markdown (GFM)  
- **Downward‑compatible**: Any MoreDown input can be rendered by a standard GFM parser without errors.  
- **Subset behavior**: Unsupported GFM constructs are passed through unparsed (plain text).

## 3. Supported Elements

| Feature              | Syntax                     | Output HTML               |
|----------------------|----------------------------|---------------------------|
| **Bold**             | `**bold**`                 | `<strong>bold</strong>`   |
| *Italic*             | `*italic*`                 | `<em>italic</em>`         |
| Inline code          | `` `code` ``               | `<code>code</code>`       |
| Link                 | `[text](https://…)`        | `<a href="…">text</a>`    |
| Line break           | Single newline             | `<br>`                    |
| ~~Strikethrough~~    | `~~text~~`                 | `<del>text</del>`         |
| Unordered list       | `- item` or `* item`       | `<ul><li>item</li></ul>`  |
| Ordered list         | `1. first` / `2. second`   | `<ol><li>first</li></ol>` |

> **List note:** Only top‑level lists are parsed. Nested lists remain as plain text.

## 4. Unsupported Elements
Any GFM syntax not listed above will remain in the output as literal text.
