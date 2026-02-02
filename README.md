# Personal Financial Control App

A cross-platform mobile application (iOS, Android & Web) built with React Native to help users manage their personal finances effectively, providing clarity and control over their spending habits.

**Keywords**: `react-native`, `finance-app`, `budgeting-app`, `expense-tracker`, `mobile-app`, `javascript`, `android`, `ios`, `financial-control`, `budget-planner`, `personal-finance`

---

## 📖 About The Project

This application was designed to solve a common problem: the lack of visibility into where one's money is going. It empowers users to track their income, plan a budget, log daily expenses, and analyze their financial behavior through an intuitive and powerful interface. By making financial data easy to understand, the app helps users make smarter decisions, identify savings opportunities, and achieve their financial goals.

The project stands out for its simplicity and focus on essential features, avoiding the complexity of many other financial tools. It's not just an expense logger; it's a personal financial assistant that brings clarity and confidence to your financial life.

To see the app in action, check out a demo video on LinkedIn:
[Watch Demo Video on LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:7424170816638111744/?originTrackingId=IXF596u%2BpD5lUJ%2FqSiSdkw%3D%3D)

<!-- Placeholder for future screenshots if needed -->
<!-- ![image](https://github.com/user-attachments/assets/e622b737-1834-4b53-8328-947700c25a58) -->


## ✨ Core Features

*   **Monthly Budget Planning**: Set your monthly income and create spending goals for different categories (e.g., Food, Transport).
*   **Daily Expense Tracking**: Quickly log expenses as they happen, assigning them to a category.
*   **Financial Analysis**: Visualize your financial health with intuitive charts and reports.
    *   A **Pie Chart** shows the percentage distribution of your expenses by category.
    *   A **Line Chart** tracks the evolution of your spending and balance over time.
*   **Smart Validation**: The app warns you if you log an expense in a category that wasn't part of your initial plan, helping maintain budget consistency.
*   **Central Dashboard**: Get an at-a-glance overview of your current balance, total income, planned expenses, and actual spending.
*   **Personalization**: Switch between light and dark themes and choose your preferred language (Portuguese/English).
*   **Persistent Local Storage**: All your financial data is securely saved on your device, ensuring it's available across sessions.

## 🚀 Technology Stack

The app is built with a modern and robust technology stack to ensure a fluid user experience and a maintainable codebase.

*   **[React Native](https://reactnative.dev/)**: Main framework for building native apps for iOS and Android from a single codebase.
*   **[React](https://reactjs.org/)**: JavaScript library for building user interfaces, serving as the foundation for React Native.
*   **JavaScript (ES6+)**: The core programming language of the application.
*   **React Context API**: Used for global state management, such as theme (light/dark) and language, avoiding "prop drilling."
*   **[AsyncStorage](https://react-native-async-storage.github.io/async-storage/)**: A persistent key-value storage system for React Native that saves user data locally on the device.
*   **[React Native Chart Kit](https://github.com/indiespirit/react-native-chart-kit)**: Library for creating beautiful charts and data visualizations.
*   **Platform API (React Native)**: Used to detect the operating system (iOS, Android) and apply platform-specific styles or components.

## ⚙️ How It Works: Application Flow

The user journey is designed to be logical and intuitive, guiding you from planning to analysis.

### 1. Planning Screen (`Planejamento.jsx`)
This is the starting point for your financial organization. Here, you can:
*   Select the month and year you want to plan for.
*   Set your monthly salary/income, which serves as the baseline for all calculations.
*   Define planned expense "goals" for the month (e.g., a maximum of $500 for Groceries).

### 2. Expense Logging Screen (`CadastroGasto.jsx`)
This screen is for recording your day-to-day expenses. You can:
*   Select the corresponding month for the expense.
*   Enter the amount, description, and category for each transaction.

### 3. Main Dashboard (`Dashboard.jsx`)
This is your financial control center, providing a comprehensive overview of the selected month. It displays:
*   **Current Balance**: Calculated as `Income - Total Spent`. The value is color-coded green (positive) or red (negative).
*   **Financial Summary**: Shows your defined income, total planned expenses, and total actual spending.
*   **Data Tabs**:
    *   **Planned Expenses**: Lists your budget goals and shows how much is still available in each category.
    *   **Actual Expenses**: Lists every transaction you've logged, with an option to filter by category.

### 4. Financial Details Screen (`DetalhamentoFinanceiro.jsx`)
Accessible from the Dashboard, this screen offers a deeper, visual analysis of your finances with:
*   **Category Analysis (Pie Chart)**: See exactly where your money went by viewing the percentage breakdown of spending per category.
*   **Temporal Analysis (Line Chart)**: Compare your total spending and final balance against previous months to track your progress.

## 🏁 Getting Started

### Download & Test (Android APK)

For a quick test on Android, you can directly download the pre-built APK file from the `apk/` directory in this repository. This allows you to install and use the application without needing to set up the development environment.

[Download the latest APK here](/apk/application-91c5d328-8455-4440-81d4-a384471f8195.apk)

To get a local copy up and running, follow these simple steps.

### Prerequisites

*   Node.js and npm
*   React Native development environment set up
    *   Follow the official guide here: [React Native Environment Setup](https://reactnative.dev/docs/environment-setup)

### Installation

1.  Clone the repo
    ```sh
    git clone https://github.com/your-username/App---Personal-Financial-Control-APK.git
    ```
2.  Install NPM packages
    ```sh
    npm install
    ```
3.  Run the application
    ```sh
    # For Android
    npx react-native run-android
    # For iOS
    npx react-native run-ios
    ```

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
