# Smart Inventory Manager 📦

> A complete inventory management system for small businesses, warehouses, and e-commerce stores. Track stock levels, automate reorders, predict demand, and manage suppliers — all in one beautiful dashboard.

## ✨ Features

- **Real-Time Stock Tracking**: Know exactly what you have, where it is, and when it expires
- **Barcode/QR Scanner**: Mobile app for instant product scanning
- **Auto-Reorder System**: Set minimum stock levels and let the system order automatically
- **Demand Forecasting**: AI predicts what you'll need based on historical data
- **Multi-Warehouse Support**: Manage inventory across multiple locations
- **Supplier Management**: Track suppliers, prices, lead times, and performance
- **Purchase Orders**: Generate and send POs directly from the system
- **Low Stock Alerts**: Get notified before you run out
- **Expiry Tracking**: Never waste products again with FIFO/FEFO management
- **Analytics Dashboard**: Visual reports on turnover, dead stock, and profitability
- **Multi-Currency**: Handle international suppliers and sales
- **Team Access**: Role-based permissions for staff

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/valentinasmith722/smart-inventory-manager.git
cd smart-inventory-manager

# Install dependencies
pip install -r requirements.txt

# Setup database
python manage.py migrate

# Create admin user
python manage.py createsuperuser

# Run the server
python manage.py runserver
```

## 📊 Dashboard Preview

```
┌─────────────────────────────────────────────────────────────┐
│  Smart Inventory Manager v3.0                                │
├─────────────────────────────────────────────────────────────┤
│  📦 Total Items: 2,847         💰 Inventory Value: $48,392  │
│  ⚠️  Low Stock: 12 items       📈 Turnover: +15% this month │
├─────────────────────────────────────────────────────────────┤
│  Stock Status Overview                                         │
│  In Stock    ████████████████████████████  2,400 (84%)      │
│  Low Stock   ████░░░░░░░░░░░░░░░░░░░░░░░    12 (0.4%)     │
│  Out of Stock██░░░░░░░░░░░░░░░░░░░░░░░░░    35 (1.2%)     │
│  Reserved    ██████░░░░░░░░░░░░░░░░░░░░░   400 (14%)      │
└─────────────────────────────────────────────────────────────┘
```

## 🛠️ Tech Stack

- **Backend**: Django 4.2 + Django REST Framework
- **Frontend**: Vue.js 3 + Vuetify + Chart.js
- **Database**: PostgreSQL + Redis (caching)
- **AI/ML**: scikit-learn + pandas (demand forecasting)
- **Mobile**: React Native (barcode scanner app)
- **Queue**: Celery + Redis (background tasks)
- **Export**: ReportLab (PDF) + openpyxl (Excel)

## 📱 Mobile App

Scan barcodes, check stock, and receive alerts on the go.

```bash
cd mobile-app
npm install
npx react-native run-android  # or run-ios
```

## 🎯 Use Cases

- **Retail Stores**: Track every product from receiving to sale
- **Restaurants**: Manage ingredients, track expiry, reduce waste
- **E-commerce**: Sync inventory across Shopify, WooCommerce, Amazon
- **Warehouses**: Multi-location stock management with pick/pack/ship
- **Manufacturing**: Raw materials, work-in-progress, finished goods
- **Pharmacies**: Track batches, expiry dates, and regulatory compliance

## 🔧 Configuration

Create a `.env` file:

```env
# Database
DATABASE_URL=postgresql://user:pass@localhost/inventory_db

# Redis
REDIS_URL=redis://localhost:6379/0

# Email (for alerts)
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=587
EMAIL_USER=your-email@gmail.com
EMAIL_PASSWORD=your-app-password

# AWS S3 (for product images)
AWS_ACCESS_KEY_ID=your_key
AWS_SECRET_ACCESS_KEY=your_secret
AWS_STORAGE_BUCKET_NAME=your_bucket

# Stripe (for supplier payments - optional)
STRIPE_SECRET_KEY=sk_test_...
```

## 📦 Core Modules

### 1. Product Management
- SKU generation and management
- Product variants (size, color, etc.)
- Images and documentation
- Categories and tags

### 2. Stock Control
- Stock in/out tracking
- Adjustments and transfers
- Cycle counting
- Audit trails

### 3. Purchase Management
- Supplier database
- Purchase orders
- Goods receipt
- Invoice matching

### 4. Sales Integration
- POS integration
- E-commerce sync
- Order fulfillment
- Returns management

### 5. Analytics & Reports
- ABC analysis
- Inventory turnover
- Dead stock identification
- Profitability by product

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Ways to Contribute

- 🐛 Report bugs via GitHub Issues
- 💡 Suggest features via GitHub Discussions
- 🔧 Submit pull requests
- 🌍 Translate to other languages
- 📖 Improve documentation

## ☕ Support This Project

This tool is **100% free and open source**. We built it to help small businesses compete with enterprise-level inventory systems without the enterprise-level price tag.

If Smart Inventory Manager helped you reduce waste, save time, or grow your business, consider supporting its continued development:

**Solana (USDT)**: `BKjS4agVRowFGqUuWHEKZerk3dCS52V1n4NdWaeNTo8E`

Your support helps us:
- Develop mobile apps for iOS and Android
- Add AI-powered demand forecasting
- Integrate with more e-commerce platforms
- Create video tutorials and documentation
- Maintain and improve the codebase
- Support small businesses worldwide

*Every contribution helps us keep this tool free for everyone. Thank you for being part of our mission.* 🙏

## 📄 License

MIT License — free to use, modify, and distribute.

## 🌟 Star History

If this project saved you time or money, please give it a star ⭐ on GitHub!

---

*Built with ❤️ for small businesses everywhere | 2026*
