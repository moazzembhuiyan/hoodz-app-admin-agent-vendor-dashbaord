<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,50:1E3A8A,100:38BDF8&height=180&section=header&text=HOODZ%20Dashboard&fontSize=40&fontColor=ffffff&fontAlignY=36&desc=Admin%20%C2%B7%20Vendor%20%C2%B7%20Agent&descAlignY=58&descSize=16" alt="HOODZ Dashboard" />

<p><b>📊 Multi-role Admin Dashboard</b></p>

<p>
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Ant_Design-0170FE?style=for-the-badge&logo=antdesign&logoColor=white" alt="Ant Design" />
  <img src="https://img.shields.io/badge/Redux_Toolkit-764ABC?style=for-the-badge&logo=redux&logoColor=white" alt="Redux Toolkit" />
  <img src="https://img.shields.io/badge/Socket.IO-010101?style=for-the-badge&logo=socketdotio&logoColor=white" alt="Socket.IO" />
  <img src="https://img.shields.io/badge/Google_Maps-4285F4?style=for-the-badge&logo=googlemaps&logoColor=white" alt="Google Maps" />
  <img src="https://img.shields.io/badge/React_Hook_Form-EC5990?style=for-the-badge&logo=reacthookform&logoColor=white" alt="React Hook Form" />
  <img src="https://img.shields.io/badge/Zod-3E67B1?style=for-the-badge&logo=zod&logoColor=white" alt="Zod" />
</p>

</div>

## 📖 Overview

A production-ready **multi-role web dashboard** for the **HOODZ** e-commerce and delivery platform. Admins, vendors and agents each get their own workspace, with **real-time updates over Socket.IO**, rider assignment on maps and full order, wallet and catalog management.

## ✨ Key Features

### ⚙️ Operations

- Dashboard stats, charts & analytics with period filters
- Order management with full status flow
- **Real-time** order updates via Socket.IO
- Find nearby riders on **Google Maps** and assign jobs
- Rider KYC review (approve / reject)
- Withdrawals, deposits & vendor settlements

### 🛍️ Catalog & Marketing

- Categories with **English / Arabic** titles
- Products with variants & stock analytics
- Campaigns, banners & vouchers
- Promotional push messages

### 🧾 Vendor Tools

- **POS** — product grid, variants, cart, discount/tax, checkout
- POS order history & payment transactions

### 💬 Support

- Live customer-support chat (typing, seen, file upload)
- Grievance resolution with compensation vouchers

## 👥 Roles

| Role | Focus |
|---|---|
| **Admin** | Users, orders, KYC, wallets, categories, campaigns, banners, settings, analytics, withdrawals, vendor payments, promotional messages |
| **Vendor** | Products, orders, POS, vouchers, transactions, shop settings |
| **Agent** | Orders, deposits, vouchers, grievances, customer & order support chat, rider assignment for unassigned orders |

## 🛠️ Tech Stack

| Category | Technology |
|---|---|
| **Framework** | Next.js 15 (App Router) · React 19 |
| **Language** | JavaScript |
| **UI** | Ant Design · Tailwind CSS · Lucide · React Icons |
| **State & API** | Redux Toolkit · RTK Query · Redux Persist |
| **Real-time** | Socket.IO Client |
| **Maps** | Google Maps API |
| **Charts** | Recharts · Chart.js |
| **Forms** | React Hook Form · Zod |
| **Editors** | Jodit · React Quill |

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ and npm

### Installation

```bash
git clone https://github.com/moazzembhuiyan/hoodz-app-admin-agent-vendor-dashbaord.git
cd hoodz-app-admin-agent-vendor-dashbaord
npm install
```

### Environment Variables

Copy the example file and fill in your values:

```bash
cp .env.example .env.local
```

```env
NEXT_PUBLIC_BASE_URL=
NEXT_PUBLIC_SOCKET_URL=
NEXT_PUBLIC_GOOGLE_MAPS_API_KEY=
```

| Variable | Description |
|---|---|
| `NEXT_PUBLIC_BASE_URL` | Backend API base URL |
| `NEXT_PUBLIC_SOCKET_URL` | Socket.IO server URL |
| `NEXT_PUBLIC_GOOGLE_MAPS_API_KEY` | Google Maps API key |

### Run

```bash
npm run dev
# open http://localhost:3000
```

## 📜 Available Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start the development server |
| `npm run build` | Create a production build |
| `npm run start` | Run the production build |
| `npm run lint` | Run ESLint |

## 📁 Project Structure

```text
src/
├── app/
│   ├── (Auth)/       # Login, OTP, password recovery
│   └── admin/        # Admin, vendor & agent pages
├── components/       # Shared UI
├── redux/            # Store & RTK Query APIs
├── context/ · hooks/
├── locales/          # Translations
├── schema/           # Zod schemas
├── theme/            # Ant Design theme
└── middleware.js     # Role-based route protection
```

## 📝 More Documentation

Detailed developer notes are available in [`docs/NOTES.md`](docs/NOTES.md).

---

<div align="center">

### 👨‍💻 Developed by [Moazzem Hossen Bhuiyan](https://github.com/moazzembhuiyan)

<sub>Mobile App Developer (React Native) • Web Developer</sub>

<p>
  <a href="https://github.com/moazzembhuiyan"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" /></a>
  <a href="https://www.linkedin.com/in/moazzem-hossen-bhuiyan-325432331/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:moazzembhuiyan394@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

<sub>⭐ If you like this project, consider giving it a star!</sub>

</div>
