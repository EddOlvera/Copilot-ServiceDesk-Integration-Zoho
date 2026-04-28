# Copilot IT Ticketing Automation

AI-driven service desk automation that converts natural language requests into structured IT tickets using Copilot Studio, Power Automate, and secure API integrations.

## Overview

This project demonstrates an end-to-end IT ticket creation workflow using Microsoft Copilot Studio and Power Automate.

The solution allows users to describe an IT issue in natural language. The Copilot agent collects the required information, generates a structured ticket subject and description, and sends the request to an external ServiceDesk system through a REST API secured with OAuth 2.0.

## Problem

Manual IT ticket creation is often inconsistent, slow, and dependent on users knowing what information to provide.

Common issues include:

- Vague ticket descriptions
- Missing required fields
- Incorrect priority selection
- Repeated follow-up questions from support teams
- Manual routing and formatting work

## Solution

The solution uses Copilot Studio as the conversational interface and Power Automate as the integration layer.

The agent collects:

- Requester email
- Issue description
- Affected service
- Priority
- Additional details
- Optional screenshot attachment

Power Automate then creates a structured IT ticket using the ServiceDesk API.

## Architecture

```text
User
  ↓
Copilot Studio Agent
  ↓
Power Automate Flow
  ↓
OAuth 2.0 Authentication
  ↓
ServiceDesk REST API
  ↓
Created IT Ticket
