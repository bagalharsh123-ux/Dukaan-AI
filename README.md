# DukaanAI 🛒 — Smart Shopkeeper Business Assistant

A fast, modern SaaS web application tailored for Indian Kirana store owners and retail shopkeepers to streamline inventory, POS billing, expense management, AI business advice, and store analytics in one unified dashboard.

---

## 🚀 Quick Start

### 1. Start Development Server
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### 2. Build for Production
```bash
npm run build
```

---

## 🛠 Tech Stack

- **Frontend:** React 18 + TypeScript + Vite
- **Styling:** Tailwind CSS (Navy `#0F172A` Sidebar, Clean `#F8FAFC` Light Mode, Emerald/Teal `#059669` accents)
- **Icons:** Lucide React
- **Data Visualizations:** Recharts (AreaChart, BarChart, Donut PieChart)
- **Persistence:** Browser `localStorage` with initial realistic demo data
- **Currency:** Indian Rupee (`₹` INR) formatting with `Intl.NumberFormat('en-IN')`

---

## 📋 Features Implemented

### 1. Dashboard (`/`)
- Top metrics: **Today's Sales**, **Low Stock Count**, **Stock Valuation**, **Today's Expenses**.
- 7-day revenue vs expense trend area chart.
- Quick action shortcuts (POS Billing, Add Product, Add Expense, Ask AI).
- Real-time recent transaction ledger.
- Urgent low stock alerts with 1-click **+10 Restock** buttons.

### 2. Inventory & Stock (`/inventory`)
- Real-time catalog with 13 pre-loaded Kirana items (Atta, Oil, Salt, Rice, Butter, Dairy, Spices, Soap, etc.).
- Search by name, category, or SKU.
- Category pills & stock status filters (All, Low Stock, Healthy Stock).
- Inline `+` / `-` stock steppers with instant persistence.
- Add & Edit Product modals with strict price and stock validations.

### 3. Sales & POS Billing (`/sales`)
- Fast Point of Sale (POS) checkout terminal.
- Product picker with stock validation (prevents overselling out-of-stock items).
- Dynamic cart calculations with discount application.
- Multi-payment support: **UPI**, **Cash**, **Udhaar / Credit**, **Card**.
- **Tax Invoice Modal:**
  - Printable receipt format (`window.print()`).
  - 1-click **"Copy for WhatsApp"** to send formatted digital bills to customers.
- Automatically decrements inventory quantities upon completing a sale!

### 4. Expenses & Khata Book (`/expenses`)
- Record business operational expenses (Rent, Electricity, Supplier Dues, Helper Wages, Tea/Snacks).
- Filter by category and date.
- Real-time expense total computation.

### 5. AI Business Assistant (`/ai-assistant`)
- Context-aware Kirana assistant that inspects **live store data**:
  - Restock analysis: Identifies all low-stock items and calculates estimated supplier capital needed.
  - Margin insights: Highlights high-margin items to boost retail profitability.
  - WhatsApp Marketing: Generates ready-to-broadcast festival promotional messages.
  - Daily summary: Summarizes today's transactions, payment breakdown, and net earnings.
  - Udhaar recovery advice: Actionable advice to settle outstanding credit bills.
- 1-click **Copy Message** button.

### 6. Analytics (`/analytics`)
- Financial overview: Total Gross Revenue, Estimated Gross Profit, Average Order Value (AOV), Operating Outflow.
- Sales by product category bar chart.
- Payment method share donut chart (UPI vs Cash vs Udhaar vs Card).
- Top-selling products leaderboard.

### 7. Settings (`/settings`)
- Store profile customization: Store name, Owner, Phone, GSTIN, Address, UPI ID, Receipt footer greeting.
- Low stock alert threshold setting.
- **Export Backup:** 1-click JSON backup download.
- **Reset Demo Data:** Revert back to fresh hackathon demo data anytime.

---

## 📱 Mobile & Responsive Design
- Responsive navigation drawer for mobile screens.
- Desktop persistent navy sidebar.
- Touch-friendly POS buttons and steppers.
