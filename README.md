# Discounted-Cashflow-Valuation
Discounted Cashflow Valuation for Public Companies
# **Financial Valuation using Discounted Cash Flow (DCF) Model**

## **Overview**
This Python script provides a **financial valuation tool** for estimating the intrinsic value of a publicly traded company using the **Discounted Cash Flow (DCF) model**. The DCF approach projects a company's future cash flows and discounts them to present value using the **Weighted Average Cost of Capital (WACC)** as the discount rate.

### **Key Features:**
- **Fetches real financial data** from Yahoo Finance (`yfinance` library)
- **Automatically calculates market value of equity** based on stock price and shares outstanding
- **Uses WACC as the discount rate**, incorporating:
  - Market capitalization (equity value)
  - Debt value
  - Cost of equity
  - Cost of debt (after tax)
- **Forecasts future cash flows** based on user-defined growth assumptions
- **Includes a terminal value calculation** to estimate long-term value
- **Outputs estimated intrinsic value per share**

## **How it Works**
1. **Retrieve financial data**: Fetch the latest stock price, shares outstanding, and cash flow.
2. **Compute WACC**: Determine the appropriate discount rate using weighted costs of equity and debt.
3. **Project future cash flows**: Grow cash flows over a set period using an assumed growth rate.
4. **Calculate terminal value**: Estimate company value beyond the forecasted years.
5. **Discount all values to present**: Convert projected values to today's dollar value.
6. **Compute intrinsic value per share**: Divide by total shares to get the final valuation.

## **Example Usage**
The script allows users to enter:
- **Stock ticker** (e.g., 'AAPL' for Apple Inc.)
- **Debt value** (total company debt)
- **Cost of equity** (expected return on equity)
- **Cost of debt** (interest rate on debt)
- **Tax rate** (corporate tax rate)
- **Initial cash flow** (latest available operating cash flow)
- **Cash flow growth rate** (assumed growth over forecast period)
- **Terminal growth rate** (assumed long-term sustainable growth)

### **Output:**
The script will return an **estimated intrinsic value per share**, helping investors determine if a stock is **overvalued or undervalued**.
