# Sales Performance Dashboard

A live sales performance tracker hosted on GitHub Pages.

## Setup

1. Create a new GitHub repo (e.g. `sales-dashboard`)
2. Upload both `index.html` and `data.json` to the root
3. Go to **Settings → Pages → Source → Deploy from branch → main → / (root)**
4. Your dashboard is live at `https://yourusername.github.io/sales-dashboard`

## Updating your numbers

All your data lives in `data.json`. Edit it directly in GitHub (click the file → pencil icon → commit).

### Update closed MRR each quarter:
```json
"closed": {
  "q1": 11417,
  "q2": 5200,   ← update this as you close deals
  "q3": 0,
  "q4": 0
}
```

### Add/edit pipeline deals:
```json
"pipeline": [
  {
    "id": 1,
    "name": "Foodliner",
    "mrr": 3500,
    "sentiment": "high"
  },
  {
    "id": 2,
    "name": "Dana",
    "mrr": 2200,
    "sentiment": "med"
  }
]
```

Sentiment options: `"high"` | `"med"` | `"low"`

## Sharing

Anyone with your GitHub Pages URL can view the live dashboard. Only you can update the data by editing `data.json` and committing.
