<div align="center">

# WealthLab

**Advanced Financial Analysis & Portfolio Management System**

![Dashboard Preview](static/dashboard.png)

</div>

**WealthLab** is a comprehensive Python-based financial analysis tool designed to help traders and investors analyze stocks using proven algorithmic strategies. It implements **Mark Minervini's Trend Template** and **Gary Antonacci's Dual Momentum** to provide actionable insights and robust portfolio management capabilities.

---

## 🚀 Key Features

*   **📊 Automatic Trend Screening**: Instantly screens stocks against **Minervini’s 8-point Trend Template** to identify high-probability setups.
*   **💪 Dual Momentum Analysis**: Calculates Relative Strength against benchmark indices (e.g., Nifty 50) and validates absolute momentum.
*   **📉 Interactive Professional Charts**: Full-screen, dark-mode interactive charts powered by Plotly, featuring moving averages, RSI, and pivot points.
*   **💼 Portfolio Management**: Track multiple portfolios, monitor daily P/L, sector allocation, and historic performance.
*   **👀 Smart Watchlist**: maintain a watchlist with automated "Upside Potential" calculations based on technical targets and momentum health.
*   **🌐 Market Breath**: Dashboard overview of market health (Bull/Bear count) to time entries effectively.

## 🛠️ Tech Stack

*   **Backend**: Python, Flask, SQLAlchemy, Pandas, NumPy
*   **Frontend**: HTML5, Tailwind CSS, JavaScript
*   **Data & Analysis**: yfinance, Plotly
*   **Database**: MySQL / SQLite (configurable)

## 📥 Installation

1.  **Clone the Repository**
    ```bash
    git clone https://github.com/vkage/WealthLab.git
    cd WealthLab
    ```

2.  **Set Up Virtual Environment** (Recommended)
    ```bash
    python -m venv .venv
    # Windows
    .venv\Scripts\activate
    # Linux/Mac
    source .venv/bin/activate
    ```

3.  **Install Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Database Configuration**
    -   Copy the example configuration file:
        ```bash
        cp .db.example mysql.db
        ```
    -   Edit `mysql.db` with your database credentials (DB_HOST, DB_USER, DB_PASSWORD, DB_NAME).

5.  **Initialize Database**
    ```bash
    python scripts/init_db.py
    ```

## ⚡ Usage

1.  **Start the Application**
    ```bash
    python app.py
    ```
    The app will start on `http://localhost:5000`.

2.  **Workflow**
    -   **Dashboard**: Check Market Breadth.
    -   **Watchlist**: Add potential candidates (e.g. `TRENT.NS`, `INFY.NS`).
    -   **Analyze**: Click "Analyze" to view detailed charts and validation status.
    -   **Portfolios**: Add purchased stocks to track performance.

## ⚠️ Disclaimer

This software is for **educational and research purposes only**. It is not financial advice. Trading stocks involves risk, and you should perform your own due diligence or consult a certified financial advisor before making any investment decisions. The developers are not liable for any financial losses.

## 📄 License

This project is licensed under the **Polyform Noncommercial License 1.0.0**.
*   **Allowed**: Personal use, modification, and self-education.
*   **Prohibited**: Commercial distribution or usage for business purposes.
