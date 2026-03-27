# Fundamentals-of-AI-and-ML
Billing Item CRUD Application – Python
# Vityarthi-Project
# 🛒 Billing Item CRUD Application – Python

A simple and efficient **Billing & Inventory Management** project that performs **CRUD operations** (Create, Read, Update, Delete) on store items. This app helps small shops or businesses manage products, update stock, and generate bills easily using pure Python. No fancy frameworks—just straightforward code that gets the job done.

---

##  Features
- **Add New Item** (Create): Quick entry for products with name, price, and quantity.
- **View All Items** (Read): Display inventory in a clean table format.
- **Update Item Details** (Update): Edit existing items on the fly.
- **Delete Items** (Delete): Remove stuff you don't need anymore.
- **Auto Bill Generation**: Pick items, add quantities, calculate subtotal + tax, and print a bill to console (easy to extend for files).
- **Data Persistence**: Stores everything in a SQLite database (`billing_items.db`)—no JSON hassle, but it's lightweight and works offline.
- **User-friendly Menu Interface**: Console-based, with screen clears and pauses for that retro feel.

---

##  Project Structure
```
billing_crud/
│
├── main.py          # The heart of the app—run this!
├── billing_items.db # SQLite DB (auto-created on first run)
└── README.md        # You're reading it!
```

---

##  Technologies Used
- **Python 3.x** (tested on 3.12+)
- **SQLite** for database storage (built-in, no installs needed)
- **Modular Functions** for clean CRUD logic
- **datetime** for bill timestamps
- No external libs—keeps it beginner-friendly and portable.

---

##  How It Works
1. **Launch the App**: Fire up `main.py` and pick from the menu.
2. **CRUD Ops**:
   - Add a product? Enter name, price, qty—total auto-calcs.
   - View list? See a formatted table with IDs, names, prices, qtys, and totals.
   - Update? Select by ID, tweak details.
   - Delete? Bye-bye item.
3. **Billing Module**:
   - Select items from inventory.
   - Specify quantities (respects stock limits).
   - Calculates: Item totals → Subtotal → 10% Tax → Grand Total.
   - Prints a nice invoice with date/time.

Data sticks around between runs thanks to SQLite. No servers, no sweat.

---

##  Sample Menu
```
🛒 BILLING & INVENTORY MANAGER
==================================================
1. Add Item
2. View Items
3. Update Item
4. Delete Item
5. Generate Bill
6. Exit
--------------------------------------------------
Pick one (1-6):
```

Example Bill Output:
```
==================================================
BILLING INVOICE
Date/Time: 2025-11-24 14:30:45
==================================================
Item                 Qty   Price
----------------------------------------
Coffee Mug           2     $12.00
Laptop               1     $999.00
----------------------------------------
Subtotal:             $1023.00
Tax (10.0%):          $102.30
Total:                $1125.30
==================================================
Thanks for shopping! 💸
```

---

##  Installation & Setup
1. **Install Python 3**: Grab it from [python.org](https://www.python.org/downloads/) if you don't have it (3.8+ works fine).
2. **Clone or Download**: 
   - Save `main.py` to a folder (e.g., `billing_crud`).
   - No Git? Just copy-paste the code into a file.
3. **Run It**:
   ```
   cd billing_crud
   python main.py
   ```
   Boom—DB auto-sets up. Add some items and bill away!

**Pro Tip**: On Windows, might need `py` instead of `python`. Tested on Linux/Mac too.

---

## 🎯 Purpose of the Project
- **Learn CRUD in Python**: Hands-on with databases without the overwhelm.
- **Data Management**: SQLite basics—query, insert, update, delete.
- **Build a Billing System**: Real-world calc logic (totals, tax) in simple functions.
- **Practice Modular Design**: Bite-sized funcs make it easy to tweak or expand.

Perfect for beginners dipping into apps, or pros prototyping fast.

---

## 💼 Applications
- **Small Shop Billing**: Track daily sales on a single machine.
- **Store Inventory Management**: Monitor stock levels crudely but effectively.
- **Product Tracking**: For hobbyists or side hustles.
- **Python CRUD Learning Project**: Great portfolio piece or classroom demo.







## 📝 License & Credits
- **License**: MIT—do whatever, just don't sue me.
- **Author**: Inspired by quick hacks; built with a bit of Grok's help.
- **Last Updated**: November 24, 2025

Questions? Hit the issues tab or just tweak the code—it's yours now. Happy billing! 🤑
