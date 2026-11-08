# Travel Agency Payment Confirmation

## Overview
This n8n workflow automates booking confirmation after a successful Stripe payment. It receives payment events through a webhook, verifies the payment status, updates the corresponding booking record, and sends a confirmation email through Gmail.

## Workflow
1. Receives a Stripe payment event through an n8n webhook.
2. Checks whether the payment status is `paid`.
3. Retrieves the matching booking using the booking reference.
4. Updates the booking status to `Paid`.
5. Sends a booking confirmation email through Gmail.

## Technologies
- n8n
- Stripe Webhooks
- n8n Data Tables
- Gmail
- Webhook Automation

## Setup Notes
After importing the workflow into n8n:
- Configure your own Gmail credentials.
- Select or recreate the required Bookings Data Table.
- Configure the Stripe webhook endpoint to send payment events to your n8n webhook URL.
- Test the workflow using Stripe test payments before using live payments.
