
# Getting started
npm install
cp .env.example .env.local   # set API + socket + map keys as needed
npm run dev


# HOODZ Admin Dashboard

A production-oriented multi-role web dashboard for the **HOODZ** e-commerce and delivery platform. Built with **Next.js (App Router)**, **React**, **Redux Toolkit Query (RTK Query)**, **Ant Design**, and **Socket.io** for realtime updates.

## Roles

| Role       | Focus                                                                                                                                |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **Admin**  | Users, orders, KYC, wallets, categories, campaigns, banners, settings, analytics, withdrawals, vendor payments, promotional messages |
| **Vendor** | Products, orders, POS, vouchers, transactions, shop settings                                                                         |
| **Agent**  | Orders, deposits, vouchers, grievances, customer/order support chat, unassigned order rider assignment                               |

## Features

### Operations

- Dashboard stats, charts, and analytics (filters by period/year)
- Order management with status flow (`pending` → `confirmed` → `processing` / Prepared → … → `delivered`)
- Realtime order list refresh via `order:updated` socket events
- Unassigned orders: find nearby riders and assign jobs over socket
- Rider KYC review (approve / reject with reason)
- Withdrawals & deposits with notes, attachments, and wallet details
- Vendor settlement payments (amount, note, optional receipt files)

### Catalog & marketing

- Category CRUD with EN/AR titles and icons
- Product management (variants, stock filters, analytics charts)
- Campaigns (products + bilingual titles)
- Banner management (`product` / `shop` / `campaign` references, sections, status toggle)
- Global / shop / compensation vouchers
- Promotional push messaging

### Vendor tools

- POS: product grid, variants, cart, discount/tax (%), checkout
- POS order history (view / delete)
- Own payment transaction history

### Agent & support

- Customer support chat (HTTP + socket: send, list, typing, seen, file upload)
- Grievance resolution (optional compensation voucher)
- Agent schedule & timezone on create/edit

### Platform

- Role-based sidebar navigation
- Central file upload hook (S3 URLs) for images/receipts
- General settings (delivery charge per km, Fawry, rider matching)
- Privacy / Terms (role-specific, read-only or editable where applicable)
- Auth layout and profile header with skeleton loading

## Tech stack

- **Framework:** Next.js (App Router), React (`"use client"`)
- **State / API:** Redux Toolkit + RTK Query (`baseApi` inject endpoints)
- **UI:** Ant Design, Tailwind CSS, Lucide icons
- **Realtime:** Socket.io client
- **Forms / UX:** dayjs, react-hot-toast, optional Chart.js / Jodit / React Quill where used
- **Auth:** JWT (e.g. `jwtDecode` for vendor shop id)

## Project structure (high level)

```text
src/
  components/     # Feature containers, modals, shared UI
  redux/api/      # RTK Query slices (orders, users, products, banner, …)
  hooks/          # e.g. useFileUpload
  context/        # Socket provider
  app/            # Next.js routes under /admin, /admin/vendor, /admin/agent
```
