# Digital-Research
# Corporate Website Quality and Stock Market Performance: FTSE 100 Evidence

This repository contains the dataset, analysis code, and results for the project “Corporate Website Quality and Stock Market Performance: Evidence from the FTSE 100,” which investigates whether and how website quality is associated with market performance in large UK-listed firms.

## Motivation

Do high-quality corporate websites translate into stock market outperformance? This research brings empirical evidence to this question, combining annual website quality scores and financial returns for FTSE 100 companies in 2024 and 2025. The study is grounded in well-established theories from finance, digital strategy, and corporate governance.

## Dataset

- **Website Quality Scores:** proprietary Black Sun's 2024 & 2025 website assessments
- **Market Performance:** FTSE 100 total stock return for 2024 & 2025
- **Controls:** firm size, industry, beta, momentum, ROA, leverage, book-to-market ratio, annual dividends
- Each analysis year includes ~100 companies with complete data (`/data` directory)

## Theoretical Framework

This research explores how corporate website quality, measured annually, relates to stock market performance among FTSE 100 firms, guided by Signaling Theory, Information Asymmetry/Disclosure Theory, the Resource-Based View (RBV), and Corporate Social Responsibility (CSR).

- **Signaling Theory:** A high-quality website demonstrates managerial credibility and acts as a signal to investors regarding the firm’s professionalism and strategic capability.
- **Information Asymmetry/Disclosure Theory:** Effective, transparent websites function as primary disclosure tools, reducing uncertainty for investors and affecting financing conditions.
- **Resource-Based View:** Website quality serves as evidence of unique, hard-to-replicate digital capabilities that can support firm competitiveness.
- **Corporate Social Responsibility:** Websites reflect a company’s commitment to transparent stakeholder engagement and ethical communication, factors increasingly linked to financial performance.

## Control Variables

- **Firm Size:** Market Capitalization (annual, 2024/2025)
- **Industry Sector:** ICB classification dummies
- **Systematic Risk:** Beta (annual)
- **Prior Performance (Momentum):** Average annual return and recent return trends (2020–2023)
- **Profitability:** Return on Assets (ROA, latest available prior year)
- **Leverage:** Debt ratio
- **Book-to-Market Ratio:** Annual book value divided by market capitalization
- **Annual Dividends:** Total dividends paid per year, as a proportion of market value

Website scores are drawn from Black Sun’s proprietary database. Financial data are sourced from Yahoo Finance and company reports.

## Research Design

- Cross-sectional regression analysis for each year (2024 and 2025)
- OLS regression:  
  - Dependent variable: TSR (2024 or 2025)
  - Independent variable: Website Quality Score (2024 or 2025)
  - Control variables: firm size, industry, beta, momentum, ROA, leverage, book-to-market ratio, annual dividends
- All results interpreted as **associations**; causality is not implied.

## Limitations

- **Endogeneity:** The cross-sectional design tests for association, not causation. Omitted factors may influence both website quality and market performance.
- **Temporal Alignment:** Website quality is measured at a specific point, while stock returns are captured over the year. Even though years are matched, some temporal misalignment is possible.
- **Sample Size:** With roughly 100 observations per year, statistical power is limited.
- **Measurement Limitations:** Website quality assessment is systematic but includes subjective judgments. Reliance on single-year stock returns may not fully capture effects on long-term value creation.
- **Potential Omitted Controls:** While efforts are made to include relevant firm-level controls (e.g., size, industry, risk, momentum, dividends, book-to-market, and leverage), not all potentially significant variables can be observed or accounted for.
- **Survivorship Bias:** Only firms with complete data are included, possibly biasing results toward more established or well-documented companies.
- **Market Environment:** Year-specific market conditions (macroeconomic or regulatory) may drive results and reduce the broader applicability of findings.

## File Structure
