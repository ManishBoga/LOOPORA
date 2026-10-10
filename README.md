# LOOPORA - Loop Optimization for Returned Assets
> **Company Return Management & Reverse Logistics Redistribution System**

LOOPORA transforms traditional e-commerce return logistics by routing customer returns to local partner hubs instead of shipping every item back to a centralized facility. Regional warehouse employees inspect products on-site:
- **Good / Restockable** items are matched and redistributed locally to fulfill nearby orders, saving freight cost, reducing transit times, and cutting carbon emissions.
- **Damaged / Unsalvageable** items are consolidated for batch transit to the central hub for repair or recycling.

---

## 🚀 Key Features

1. **Executive Dashboard**:
   - Real-time KPIs: *Total Returns, Inspected, Ready for Resale, Total Savings (₹)*.
   - Interactive charts with Recharts: *Weekly Returns Volume (Mon–Sun)* and *Return Reasons Breakdown (Donut)*.
   - Recent Returns live table.

2. **Upload JSON (Batch Ingestion)**:
   - Import company returns manifests in bulk via `.json`.
   - File validation, data schema mapping, and live table preview.

3. **Returns Master Registry**:
   - Searchable database of all returns with real-time text query.
   - Status indicators (`Received`, `Inspection`, `Ready`, `Redistributed`, `Sent to Central`).
   - Action to move incoming returns into the inspection pipeline.

4. **Inspection Station**:
   - Warehouse ground staff verification queue.
   - One-click condition assignment: **Good / Ready** vs **Damaged / Sent to Central**.

5. **Local Redistribution Engine**:
   - Pairs `Ready` products with pending nearby customer orders.
   - Computes logistics cost savings per item.
   - One-click **Assign Delivery** dispatching.

6. **Stock Overview**:
   - Inventory matrix across core products (*Dell Laptop, iPhone 13, Boat Earphones, Men Jacket, Women Dress, Samsung Mobile*).
   - Real-time count of good vs damaged stock with automated recommendations (*Keep for local resale* vs *No local stock*).

7. **Warehouse Employee Roster**:
   - Multi-hub employee directory: Hyderabad Hub, Delhi West, Mumbai Central, Bengaluru South.

8. **Impact Reports**:
   - Environmental and cost metrics: good items reused locally, items sent to central, total ₹ saved.

---

## 🛠️ Tech Stack

- **Frontend**: React 18, Vite
- **Data Visualization**: Recharts
- **Icons**: Lucide React
- **Styling**: Modern responsive CSS with custom design system
- **State & Data**: Reactive `localStorage` (default offline demo mode) + optional Cloud Firestore & Firebase Auth

---

## 💻 Quick Start

### 1. Install dependencies
```bash
npm install
```

### 2. Run local development server
```bash
npm run dev
```

### 3. Build for production
```bash
npm run build
```

---

## 🔑 Login Credentials (Demo Mode)

- **Email**: `employee@loopora.com`
- **Password**: `123456`

*(Works offline without any cloud configuration. To connect to a live Firebase backend, create a `.env` file with your Firebase project keys)*.
