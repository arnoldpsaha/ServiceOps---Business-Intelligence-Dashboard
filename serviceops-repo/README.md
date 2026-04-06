# ServiceOps IE Dashboard

Mobile-first business intelligence dashboard for service businesses in the Inland Empire.

## How to update data

1. Export a fresh CSV from your platform (Jobber, QuickBooks, etc.)
2. Go to the `data/` folder in this repo
3. Click the file you want to update
4. Click the pencil icon to edit
5. Select all → paste your new CSV content → Commit

The dashboard fetches these files live every time the page loads.

## File map

| File | Source platform | Updates |
|------|----------------|---------|
| `data/jobber_jobs.csv` | Jobber → Jobs → Export | Weekly |
| `data/quickbooks_invoices.csv` | QuickBooks → Reports → Sales by Customer | Weekly |
| `data/hubspot_contacts.csv` | HubSpot → Contacts → Export | Weekly |
| `data/google_ads_campaigns.csv` | Google Ads → Campaigns → Download report | Weekly |
| `data/optimoroute_stops.csv` | OptimoRoute → Planning → Export Stops | Daily |

## Folder structure

```
serviceops-dashboard/
├── index.html
├── README.md
└── data/
    ├── jobber_jobs.csv
    ├── quickbooks_invoices.csv
    ├── hubspot_contacts.csv
    ├── google_ads_campaigns.csv
    └── optimoroute_stops.csv
```
