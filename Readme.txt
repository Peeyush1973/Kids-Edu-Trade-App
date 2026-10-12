Kids Edu Trade Learning App

A gamified stock trading simulator built for kids and beginners to learn investing in a safe, risk free environment. The app uses virtual money, real market data, and interactive learning tools to teach core financial concepts through hands on practice rather than theory.

Overview

EduTrade is a Unity based paper trading application designed to introduce young learners and complete beginners to the stock market. Users start with a virtual wallet of ten thousand virtual dollars and can buy and sell real NIFTY 50 stocks at live prices. Every action is guided, explained, and rewarded with experience points, levels, and achievements so learning feels like a game.

The goal is simple. Before risking real money, understand how markets work. Learn what a stock is, why prices move, what risk means, and how discipline and diversification protect a portfolio. EduTrade gives users that knowledge through practice.

Key Features

Live market data. The app fetches real time prices for NIFTY 50 companies using Yahoo Finance. When offline, it falls back to simulated prices so the learning never stops.

Interactive candlestick charts. Users can zoom, pan, draw trend lines, place horizontal price markers, measure price moves with a ruler tool, and toggle indicators like SMA20, volume bars, and grid lines.

Candlestick pattern detection. The chart identifies patterns like Doji, Hammer, Bullish and Bearish Engulfing, Morning Star, Evening Star, Three White Soldiers, and Three Black Bears in real time. Each detected pattern is annotated directly on the chart and explained in a dedicated info panel with what it means and what to watch for.

Full order system. Market buy, market sell, limit buy, limit sell, and stop loss orders are all supported. Pending orders wait for their trigger price and execute automatically.

Trade panel with quantity controls. A bottom sheet interface lets users adjust order size, see required margin as a percentage of available cash, set take profit and stop loss levels, and preview the exact price before confirming.

Portfolio tracking. Every holding is tracked with average buy price, live value, and profit or loss. Portfolio value over time is drawn as a line chart, and allocation by symbol is shown as a pie chart.

Learning center. Structured lessons cover foundations, portfolio theory, charts, and trading. Each completed lesson awards experience points and unlocks achievements.

Interactive quiz system. After every fifth trade, a quiz pops up related to what the user just did. Wrong answers are explained in detail so the lesson is not lost.

Trade journal. Every trade is logged with an optional reflection tag so users can look back and understand what worked and what did not.

Daily rewards. Users receive bonus cash and experience for logging in each day, with a streak multiplier for consecutive days.

Achievements. Unlockable badges for milestones like first trade, diversified portfolio, ten trades, five completed lessons, and consistent daily streaks.

AI assistant. A built in chat assistant answers questions about stocks, trading concepts, and how to use the app. It works entirely offline with a curated knowledge base so no API key or internet connection is required.

Onboarding tour. First time users are guided through the app with an interactive spotlight tour that highlights each section and can be skipped or restarted at any time.

Themes and accessibility. Dark mode and light mode are both supported. A colorblind mode swaps the traditional red and green for colors that are easier to distinguish. Font size can be scaled up or down for readability.

Sound effects. Optional buy, sell, achievement, and alert sounds make every action feel responsive.

Responsive design. The entire interface adapts to desktop, tablet, and phone screen sizes. On phones the sidebar collapses into a drawer, a bottom navigation bar appears, and every interactive element is sized to the recommended touch target for comfortable use.

How It Works

When a user opens the app for the first time, they are greeted by a tutorial that walks them through the dashboard, market, portfolio, and learning pages. From there they can:

Browse the market, filter stocks, and add favourites to a watchlist.

Click any stock to see its live price chart, candlestick patterns, and order book.

Place a trade using the buy or sell button, which opens a full order sheet.

Watch their portfolio value update in real time as prices move.

Complete lessons and quizzes to earn experience and unlock achievements.

Review their trading history in the journal and their overall progress in the recap screen.

Everything happens with virtual money, so mistakes cost nothing and every decision is a learning opportunity.

Technology Stack

Unity game engine for cross platform builds.

UI Toolkit for the entire user interface, built with UXML and USS.

C# for all application logic.

Yahoo Finance public API for real time market data.

Persistent save system written to the device as JSON.

Fully offline assistant powered by a curated knowledge base.

Project Structure

The project is organised under Assets/TradingLearningApp with clear separation between runtime logic and editor tooling.

Runtime Core contains the app controller, state management, persistence, notifications, theme control, audio, and the shell controller that wires the entire UI together.

Runtime Market contains the market data services, trade service, order service, portfolio service, chart controller, chart tools, order book, pattern detector, portfolio charts, and the trade panel controller.

Runtime Learning contains the lesson catalog, lesson controller, and quiz logic.

Runtime Assistant contains the offline knowledge base and the chat controller.

Runtime Rewards contains the daily reward controller.

UI AppShell contains the single UXML file and USS file that define the entire interface.

Editor contains the setup tool that configures the scene in one click and helper utilities.

Getting Started

To run this project, install Unity 2022 LTS or later with the Android Build Support module if you plan to build for Android.

Open the project in Unity Hub, then run the menu command Tools, Trading Learning App, Setup Complete Trading App. This creates the main game object, attaches every controller, assigns the UXML file, and prepares everything for play.

Press Play in the editor to test the app.

To build for Android, switch the platform to Android in Build Settings, configure the package name to a unique identifier, set the scripting backend to IL2CPP, enable ARM64 architecture, and build. The app will install on any modern Android device.

To build for Windows or Mac, switch to the corresponding platform and build normally.

Requirements

Unity 2022.3 LTS or newer.

Android SDK and NDK for Android builds.

Internet connection on first launch to fetch live market data. The app continues to work offline afterwards.

Roadmap

Additional lessons on fundamental analysis and valuation.

Portfolio rebalancing tools.

More advanced chart indicators like RSI and MACD.

Multiplayer challenges and leaderboards.

Cloud save support.

Localisation into additional languages.

License

This project is released under the MIT License. You are free to use, modify, and distribute it for personal or educational purposes.

Acknowledgements

Market data provided by the public Yahoo Finance API.

Candlestick pattern detection logic inspired by classical technical analysis literature.

Built with a focus on teaching, not just trading.

Contact

For questions, suggestions, or collaboration, open an issue on the GitHub repository or reach out directly through the contact information listed on the profile.

Learning to invest should be safe, guided, and fun. EduTrade exists to make that possible.