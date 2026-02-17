# Stock Price Trend Analyzer

[![Python Version](https://img.shields.io/badge/python-3.7%2B-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> A Python tool for identifying and visualizing the price trend of a stock.

This application helps investors understand whether a stock is in an uptrend, downtrend, or moving sideways by analyzing its moving averages.

## Table of Contents

- [Trend Analysis Logic](#trend-analysis-logic)
- [How to Interpret the Graph](#how-to-interpret-the-graph)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Trend Analysis Logic

The trend is determined using a combination of moving averages and slope calculation:

-   **Moving Averages (MA)**: Two moving averages are calculated:
    -   A short-term moving average (20 days).
    -   A long-term moving average (50 days).
-   **Slope Calculation**: The slope of the long-term moving average is computed.
    -   If the slope is positive and above a certain threshold, the stock is considered to be in an **uptrend**.
    -   If the slope is negative and below a certain threshold, it's a **downtrend**.
    -   Otherwise, the trend is **sideways**.

## How to Interpret the Graph

The generated graph provides a visual representation of the trend:

-   **Blue line**: The stock's closing price.
-   **Orange line**: The short-term moving average (20 days).
-   **Green line**: The long-term moving average (50 days).
-   **Title**: Displays the detected trend (Uptrend, Downtrend, or Sideways).

## Tech Stack

-   Python
-   yfinance
-   pandas
-   numpy
-   matplotlib

## Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/AbhiramSharma/Stock-Price-Trend-Analyzer.git
    cd Stock-Price-Trend-Analyzer
    ```

2.  **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  Run the analyzer from your terminal:
    ```bash
    python trend_analyzer.py
    ```

2.  When prompted, enter the stock symbol you want to analyze (e.g., `AAPL`).

## Contributing

Contributions are welcome! If you have ideas for new features or improvements, feel free to fork the repository and submit a pull request.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.

## Contact

Abhiram Sharma - ab23.ar39@gmail.com

Project Link: [https://github.com/AbhiramSharma/Stock-Price-Trend-Analyzer](https://github.com/AbhiramSharma/Stock-Price-Trend-Analyzer)
