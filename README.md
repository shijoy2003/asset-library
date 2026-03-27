# Asset Checkout System (Laptops & Peripherals)

## Project Overview
A Power Apps solution to manage asset inventory and track temporary checkouts of laptops and peripherals.

## Business Problem
Maintain a simple asset register and track temporary check-outs to prevent loss and manage inventory efficiently.

## Tools Used
- Microsoft Power Apps (Model-driven app)
- Microsoft Dataverse
- Power Automate
- Microsoft Teams

## Tables
### Assets
| Column | Type |
|--------|------|
| Asset Tag | Text |
| Model | Text |
| Category | Choice (Laptop, Monitor) |
| Status | Choice (Available, Checked Out, In Repair) |
| Condition | Choice (New, Good, Damaged) |

### Asset Checkout
| Column | Type |
|--------|------|
| Asset | Lookup (Assets table) |
| Assignee | Text |
| Checkout Date | Date |
| Due Date | Date |
| Returned On | Date |

## Features
- Asset register with 100 sample assets
- Checkout tracking with due dates
- Automatic daily reminder 24 hours before due date
- Teams notification to assignee
- Prevent double checkout rule
- Overdue items view
- Analytics chart for utilization by asset type

## Power Automate Flows
1. **Asset Due Date Reminder** - Runs daily, sends email and Teams notification to assignee 24 hours before due date
2. **Prevent Double Checkout** - Blocks checkout if asset is already checked out

## App Link
[https://org4f82fe4e.crm.dynamics.com/main.aspx?appid=2418af17-ff27-f111-8341-6045bd0125a6]

## Screenshots
See screenshots folder for app demo images.
