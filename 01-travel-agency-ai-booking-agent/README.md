# Travel Agency AI Booking Agent

## Overview
An AI-powered travel booking assistant built with n8n, Google Gemini, Stripe, and Gmail. It helps customers explore tours, check availability, make reservations, receive Stripe payment links, and get booking-related email notifications.

## Key Features
- Conversational AI travel assistant.
- Provides tour information and pricing.
- Checks tour availability and remaining seats.
- Collects customer booking details.
- Stores booking information in an n8n Data Table.
- Generates Stripe payment links.
- Sends payment links to customers through Gmail.
- Tracks bookings awaiting payment.

## Workflow
1. Customer interacts with the AI travel assistant.
2. AI provides tour details and checks availability.
3. Customer selects a tour and provides booking information.
4. Booking details are stored in the Data Table.
5. A Stripe payment link is generated.
6. Gmail sends the payment link to the customer.
7. Booking remains pending until payment confirmation.

## Technologies Used
- n8n
- Google Gemini
- Stripe
- Gmail
- JavaScript
- AI Agents
- Webhooks
- Data Tables

## Project Purpose
To demonstrate how AI agents can automate travel inquiries, tour selection, reservation management, payment processing, and customer email communication.

## Related Workflow
The separate **Payment Confirmation Webhook** handles successful Stripe payments, updates booking status, and sends booking confirmation emails through Gmail.
