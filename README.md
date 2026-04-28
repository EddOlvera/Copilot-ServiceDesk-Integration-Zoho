# Copilot IT Ticketing Automation

AI-driven service desk automation that converts natural language requests into structured IT tickets using Copilot Studio, Power Automate, and secure API integrations.

---

## Overview

This project demonstrates an end-to-end IT ticket creation workflow using Microsoft Copilot Studio and Power Automate.

The solution allows users to describe an IT issue in natural language. The Copilot agent collects the required information, generates a structured ticket subject and description, and sends the request to an external ServiceDesk system through a REST API secured with OAuth 2.0.

---

## Problem

Manual IT ticket creation is often inconsistent, slow, and dependent on users knowing what information to provide.

Common issues include:
- Vague ticket descriptions
- Missing required fields
- Incorrect priority selection
- Repeated follow-up questions
- Manual routing and formatting work

---

## Solution

The solution uses Copilot Studio as the conversational interface and Power Automate as the integration layer.

---

## Architecture

User → Copilot → Power Automate → OAuth → ServiceDesk API → Ticket Created

---

## Key Features

- Natural language IT ticket creation
- Dynamic subject and body generation
- OAuth 2.0 authentication
- REST API integration
- Template-based ticket creation
- Custom field mapping (UDF)
- Ticket ID + URL response

---

## OAuth 2.0 Flow

Initial:
authorization_code → access_token + refresh_token

Runtime:
refresh_token → new access_token → API request

---

## Known Challenges

UPLOAD_RULE_NOT_CONFIGURED

Attachments require ServiceDesk configuration.

---

## Project Status

Ticket creation: Working
OAuth: Working
Attachments: Blocked (config)

---

## Author

Eduardo Olvera
