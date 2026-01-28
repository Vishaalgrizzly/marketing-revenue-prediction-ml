# Marketing Revenue Prediction Model

### About the Author
**MSc Digital Marketing & AI Student | SKEMA Business School**
Passionate about bridging the gap between creative marketing strategy and data-driven decision making. This project represents my work in applying Machine Learning to optimize marketing budgets.

--- xxx ---

### Project Overview
This project applies **Linear Regression (Machine Learning)** to a dataset of digital marketing campaigns. The goal was to build a predictive model that allows marketing managers to identify which channels, devices, and campaign types drive the highest Revenue.

**The Business Problem:**
Marketing teams often track metrics like "Impressions" or "Spend," but these don't always correlate with financial success. This model isolates the variables that *actually* drive revenue to answer questions like:
* *Do "Promo" campaigns drive profit, or just cheap traffic?*
* *Is Mobile traffic worth the same investment as Desktop traffic?*

### Key Insights & Business Logic
The model achieved an **R² score of 0.96**, meaning it explains 96% of revenue variance. By analyzing the coefficients, I derived the following strategic insights:

**1. The "Brand" vs. "Promo" Paradox**
* **Brand Campaigns (+267€ Impact):** Campaigns focusing on brand equity are high-value drivers.
* **Promo Campaigns (-163€ Impact):** Despite potentially higher volume, "Promo" campaigns showed a negative correlation with revenue efficiency compared to the baseline.
* *Strategy:* Shift budget from deep-discount promos to brand-building activities to maximize AOV (Average Order Value).

**2. Device Valuation**
* **Desktop (+203€):** The most valuable user segment.
* **Mobile (-96€):** Mobile traffic underperforms significantly in revenue generation.
* *Strategy:* Retain Mobile for awareness/reach, but prioritize Desktop for conversion-focused bidding strategies.

**3. The Efficiency Trap**
* **Conversions (+1,139€):** The strongest predictor of revenue (naturally).
* **Spend (-51€):** When controlling for conversions, increased Spend has a *negative* coefficient. This highlights that "spending more" without maintaining conversion rates actually hurts ROI.

### 🛠️ Technical Implementation
* **Language:** Python 3.x
* **Libraries:** Pandas, Scikit-Learn, Matplotlib
* **Methodology:**
    * **Preprocessing:** `OneHotEncoder` for categorical variables (Device, Campaign Type), `StandardScaler` for numerical scaling.
    * **Pipeline:** Implemented a Scikit-Learn `Pipeline` to ensure reproducible data transformation.
    * **Model:** Linear Regression to quantify the exact financial impact (coefficient) of each feature.

### How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/](https://github.com/vishaalgrizzly/marketing-revenue-prediction-ml.git
