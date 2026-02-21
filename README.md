# 💰 Money Manager App — Complete Android Project

A complete personal finance Android app built with Java + Room Database.

---

## 📱 Features
- **Dashboard** — Balance overview, income/expense summary, pie chart, recent transactions
- **Transactions** — Add/view all income & expenses with categories
- **Accounts** — Multiple wallets (Cash, Bank, GCash, etc.) with color coding
- **Budget Planner** — Set monthly budgets per category with progress bars
- **Savings Goals** — Track savings goals with deadlines and progress
- **Bills** — Manage recurring bills with paid/unpaid status
- **Reports** — Pie chart and bar chart for spending analysis
- **Bill Reminders** — Daily background notifications for upcoming bills

---

## 🛠️ Tech Stack
| Tool | Purpose |
|------|---------|
| Java | Programming language |
| Room Database | Local data storage |
| LiveData + ViewModel | Reactive UI updates |
| RecyclerView | Lists |
| MPAndroidChart | Charts & graphs |
| WorkManager | Background bill reminders |
| Material Design 3 | Beautiful UI components |

---

## 🚀 How to Open in Android Studio

1. **Open Android Studio**
2. Click **"Open"** or **"File > Open"**
3. Navigate to and select the **MoneyManager** folder
4. Wait for Gradle sync to complete (first time takes a few minutes)
5. Click the **▶ Run** button (or Shift+F10)

> **Note:** You need internet on the first build so Gradle can download the libraries.

---

## 📁 Project Structure

```
MoneyManager/
├── app/
│   ├── src/main/
│   │   ├── java/com/moneymanager/app/
│   │   │   ├── database/
│   │   │   │   ├── entity/          ← Data models (Account, Transaction, etc.)
│   │   │   │   ├── dao/             ← Database queries
│   │   │   │   └── AppDatabase.java ← Room database setup
│   │   │   ├── ui/
│   │   │   │   ├── activities/      ← All screens
│   │   │   │   ├── fragments/       ← Dashboard, Transactions, Accounts, etc.
│   │   │   │   └── adapters/        ← RecyclerView adapters
│   │   │   └── utils/
│   │   │       ├── AppUtils.java         ← Helper methods
│   │   │       └── BillReminderWorker.java ← Notification worker
│   │   ├── res/
│   │   │   ├── layout/              ← All XML screen layouts
│   │   │   ├── values/              ← Colors, strings, themes
│   │   │   └── drawable/            ← Icons and shapes
│   │   └── AndroidManifest.xml
│   └── build.gradle                 ← Dependencies
└── build.gradle                     ← Project config
```

---

## 💡 Tips for Beginners

- **Run the app** on an emulator (AVD Manager) or physical Android device
- **To add your first account**: Go to Accounts tab → tap the + button
- **To record a transaction**: Tap the + (FAB) button on Dashboard or Transactions tab
- **Budget tracking**: Budget section shows how much you've spent vs. your limit
- **Bill reminders**: App will notify you 3 days before a bill is due

---

## 🔧 Customization

To change the **currency** from Philippine Peso (₱) to another:
Open `utils/AppUtils.java` and change:
```java
new Locale("en", "PH")  // Change "PH" to your country code
```
Example: `new Locale("en", "US")` for US Dollars ($)

---

## 📦 Dependencies (auto-downloaded by Gradle)
- Room 2.6.1
- MPAndroidChart v3.1.0
- Material Components 1.11.0
- WorkManager 2.9.0
- RecyclerView 1.3.2
