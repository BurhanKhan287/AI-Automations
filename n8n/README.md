# n8n Automations

This directory contains reusable n8n workflows.

## Organization

```text
n8n/
├── ai-receptionist/          # Voice/AI receptionist workflows
├── ecommerce/                # E-commerce and product-data workflows
└── README.md
```

## Naming convention

Use lowercase, descriptive names with hyphens:

`<use-case>-<purpose>.json`

Examples:

- `ai-receptionist/lead-booking.json`
- `ecommerce/product-ingestion-rag.json`

## Importing a workflow

1. Open n8n.
2. Select **Import from File**.
3. Choose the `.json` workflow file.
4. Reconnect credentials and environment-specific services.
5. Test the workflow before activating it.

> Credentials are not stored in this repository. Configure your own credentials in n8n after importing a workflow.
