# 📰 News Data - Flat File Dataset

A simple flat file dataset containing news articles across multiple categories, ready to use in web or mobile projects.

---

## 📁 Files

| File | Format | Description |
|------|--------|-------------|
| `data.json` | JSON | Full dataset in JSON array format |
| `data.csv` | CSV | Full dataset in comma-separated format |

---

## 📊 Dataset Overview

- **Total Articles:** 21
- **Fields:** `id`, `title`, `description`, `image`, `category`
- **Image Source:** [Unsplash](https://unsplash.com)

---

## 🗂️ Categories

| Category | Count |
|----------|-------|
| Technology | 5 |
| Business | 4 |
| Politics | 4 |
| Sports | 4 |
| Entertainment | 4 |

---

## 🧩 Data Structure

### JSON
```json
[
  {
    "id": 1,
    "title": "Article Title",
    "description": "Short description of the article.",
    "image": "https://images.unsplash.com/photo-xxxxx",
    "category": "Technology"
  }
]
```

### CSV
```
id,title,description,image,category
1,Article Title,Short description.,https://images.unsplash.com/photo-xxxxx,Technology
```

---

## 🚀 How to Use

### JavaScript (fetch JSON)
```javascript
fetch('data.json')
  .then(res => res.json())
  .then(data => console.log(data));
```

### JavaScript (filter by category)
```javascript
const tech = data.filter(item => item.category === 'Technology');
```

### Python (read CSV)
```python
import pandas as pd
df = pd.read_csv('data.csv')
print(df.head())
```

### Python (read JSON)
```python
import json
with open('data.json') as f:
    data = json.load(f)
```

---

## 📌 Notes
- Images are hosted on Unsplash (free to use)
- All descriptions are short and suitable for card-style UI layouts
- IDs are sequential starting from 1

---

## 📄 License
Free to use for personal and educational projects.
