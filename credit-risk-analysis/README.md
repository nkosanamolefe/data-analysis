# Credit Risk Report

## **Client Background**

Nova Bank is a diversified financial institution providing a range of loan products including personal, medical, education, and business loans across the United States, United Kingdom, and Canada. The bank's primary objective is to balance fair and accessible lending with robust risk management. In the current economic climate of late 2025, with rising interest rates, precise and dynamic risk assessment is more critical than ever to maintain a healthy and competitive lending portfolio.

Nova Bank's key challenge is to optimize its lending decisions. Overly permissive lending can lead to financial losses from defaults, while overly strict criteria can result in missed opportunities and alienated potential customers. This analysis aims to provide data-driven insights to help Nova Bank refine its lending policies for both improved safety and fairness.

Nortstar Metrics

## **Executive Summary**

This report presents a comprehensive credit risk analysis of Nova Bank's $312 million loan portfolio. The analysis reveals a significant **portfolio-wide default rate of 21.82%**, resulting in over **$77 million in defaulted loan value**. The findings indicate that this risk is not uniformly distributed but is highly concentrated within specific, identifiable borrower segments and loan structures.

This analysis of Nova Bank's $312.43 million loan portfolio, comprising 33,000 loans, reveals a significant credit risk exposure, with an overall **default rate of 21.82%** by loan count and a **financial loss rate of 24.69%**, amounting to over **$77 million in defaulted loan value**. Our findings indicate that credit risk is not evenly distributed across the portfolio; rather, it is highly concentrated and predictable based on specific loan and borrower characteristics.

**Key Findings:**

1.  **A Clear Profile of the High-Risk Borrower Has Emerged.** Default is heavily concentrated among borrowers with specific demographic and behavioral traits. The most powerful predictors are **home ownership status** (renters default at over 4 times the rate of owners) and **low income** (individuals earning under $25k, particularly those aged 45-61, have default rates exceeding 60%). A history of even **one past delinquency** dramatically increases the probability of future default. Conversely, factors like employment type and geographic location show minimal correlation with risk.

2.  **The Bank’s Own Loan Structure is a Primary Driver of Default.** Nova Bank's internal loan grading system is a powerful but alarming predictor of risk. **Grade D represents a critical tipping point**, where the default rate skyrockets from 21% (Grade C) to **59%**. Grades F and G are financially unsustainable, with near-total loss rates. Furthermore, the **Loan-to-Income (LTI) ratio** is a critical affordability metric; risk accelerates exponentially as the LTI exceeds 0.4, indicating that the bank is originating loans that are fundamentally unaffordable for a significant segment of its borrowers.

3.  **Loan Purpose and Interest Rates Tell a Story of Financial Distress.** Loans taken for **Debt Consolidation** and **Medical** needs carry the highest risk, suggesting they are often loans of necessity rather than opportunity. This is compounded by the fact that borrowers in the highest interest rate brackets (20%+) have an **85% default rate**, confirming that while the bank is correctly identifying risk, the pricing is insufficient to cover the near-certain losses.

4.  **Proactive Intervention is Both Possible and Necessary.** We have developed an early warning system that has identified **122 active accounts** currently exhibiting clear signs of imminent financial distress. These individuals are characterized by a combination of prior delinquencies, high Credit Utilization (~70%), and unsustainable Debt-to-Income ratios (>43%). These accounts represent a clear opportunity to move from reactive loss collection to proactive risk mitigation.

## **Dataset**

Dataset provided by Nova Bank, contains over 32k individual loan records, each described by over 35 distinct fields. These fields encompass a comprehensive range of information, including borrower profile, loan characteristics (purpose, amount, grade), and key financial health indicators such as debt-to-income ratios and credit history.

## **Insights Deep-Dive**

###  **Borrower Risk Profile**

An analysis of borrower demographics and behavioral history reveals a set of powerful, interlocking patterns that define credit risk. While some traditional assumptions hold true, others are challenged by the data.

#### **Home Ownership: The Clearest Divide Between Safe and Risky**

The single most powerful demographic predictor of default is home ownership status. The data shows a stark and unambiguous divide between borrowers who own property and those who do not, making this a cornerstone indicator for risk assessment.

*   **High-Risk Segment:** Borrowers who **rent (32%)** or fall into the **"Other"** category (31%) exhibit exceptionally high default rates. This group represents a clear and significant risk to the portfolio.
*   **Low-Risk Segment:** In stark contrast, **homeowners who own outright (7%)** and those with a **mortgage (13%)** are substantially more reliable. The default rate for outright owners is over four times lower than for renters, suggesting property ownership is a strong proxy for financial stability.

#### **The Critical Interplay of Age and Income**

Default risk is not driven by age or income in isolation, but by their critical interaction. The analysis pinpoints low-income brackets as the primary source of portfolio risk, a vulnerability that is especially pronounced in middle-aged borrowers.

*   **The Low-Income Hazard Zone:** Borrowers earning **less than $25,000 per year consistently have the highest default rates**, frequently exceeding 50%. The risk peaks in the **45-54 age bracket, where 61% of low-income borrowers default**.
*   **Income as the Great Mitigator:** As income rises, default risk plummets across all age groups. Reaching an income of $50k-$100k typically cuts the default risk by more than half compared to the lowest bracket, confirming that repayment ability is fundamentally tied to income level.

#### **Past Delinquencies: A Clear Behavioral Warning**

A borrower's history of meeting their obligations is a powerful predictor of future behavior. The data shows a direct relationship between the number of past delinquencies and the likelihood of a new default.

*   **Escalating Risk:** While borrowers with zero past delinquencies have a baseline default rate of 22%, the risk begins to climb with each subsequent instance of non-payment, reaching **25% for those with five past delinquencies**.
*   **The Warning Sign:** A history of delinquency, regardless of the number, flags a borrower as having a higher-than-average risk profile compared to someone with a clean record in a similar financial position.

#### **The Surprising Myth of Employment Stability**

Contrary to conventional wisdom, a borrower's employment status—whether full-time, part-time, self-employed, or unemployed has a negligible impact on their likelihood to default.

*   **A Negligible Difference:** The default rates for all employment categories are clustered in an extremely narrow band between **22% and 23%**. This indicates that the employment *label* is not a meaningful differentiator of risk.
*   **Income, Not Status, is Key:** This finding strongly suggests that the *level and stability of a borrower's income* are far more important than their employment classification. A high-income, self-employed individual is a better risk than a low-income, full-time employee.

### **Loan Characteristics Analysis**

#### **Loan Grade Risk Matrix: The Breaking Point is Clear**

The bank’s internal loan grading system is not just a predictor; it is a stark dividing line between manageable risk and near-certain loss. The data validates the model's accuracy while simultaneously sounding an alarm about the extreme risk concentrated in the lower grades.

*   **The Grade D Cliff:** While Grades A, B, and C show a predictable, incremental increase in default (from 10% to 21%), **Grade D represents a catastrophic breaking point**. The default rate skyrockets to **59%**, and the financial loss rate mirrors this at 58%.
*   **Unsustainable Lower Grades:** Lending to grades E, F, and G is financially untenable. **Grade G loans have a staggering 98% default rate and a 100% loss rate**, meaning every dollar lent to this segment is lost, despite the high average interest rate of 20%.

#### **Loan-to-Income Ratio: The Affordability Threshold**

The Loan-to-Income (LTI) ratio is the single most important measure of a loan's affordability. The analysis shows that as the loan amount becomes a larger portion of a borrower's income, the risk of default doesn't just increase—it accelerates exponentially.

*   **Accelerating Risk:** The default rate climbs from a manageable 13% for LTI ratios under 0.2 to 36% for ratios between 0.2 and 0.4.
*   **The Point of No Return:** Beyond an LTI of 0.4, affordability collapses. The default rate more than doubles, jumping to **75%**. This is the critical threshold where loans become fundamentally unsustainable for the borrower.

#### **Loan Interest Rate Impact: Pricing for Risk vs. Inviting Default**

The bank’s risk-based pricing model functions as intended—higher-risk borrowers are assigned higher rates. However, the data reveals that for the highest-risk segments, the interest rate premium is wholly insufficient to compensate for the overwhelming probability of default.

*   **Volume vs. Risk:** The majority of the bank's loans (and lowest defaults at 11%) are issued at rates below 10%. As the interest rate increases, loan volume plummets while risk soars.
*   **Extreme Risk in High-Rate Loans:** Borrowers in the 15-20% interest rate bracket have a **57% default rate**. For those with rates of 20% or more, the default rate reaches an astonishing **85%**.

#### **Loan Term: A Non-Linear Risk Curve**

The relationship between loan term and default risk is more complex than a simple "longer is riskier" assumption.

*   **The 24-Month Anomaly:** Risk is lowest for 12-month loans (20%) but unexpectedly peaks early at **22% for 24-month terms**. This suggests a specific, riskier borrower profile may be drawn to this particular term.
*   **Long-Term Risk:** The default rate dips slightly for 36-month loans before climbing back to 22% for 60-month terms, confirming that longer-term exposure does ultimately correlate with higher risk.

### **Early Warning Indicators**

To transition from reactive loss recovery to proactive risk mitigation, Nova Bank has developed an early warning system designed to identify active borrowers exhibiting clear signs of financial distress. This system has flagged **122 accounts** as "High-Risk Profiles" that warrant immediate, targeted intervention. An analysis of this cohort reveals a consistent and dangerous pattern of financial instability, providing a clear blueprint for action.

#### **Anatomy of a High-Risk Profile**

The 122 identified borrowers are not defined by a single metric but by a powerful combination of four critical characteristics. This "syndrome" of financial distress makes them highly susceptible to default.

1.  **Universal Delinquency:** The most definitive red flag is a **100% rate of prior delinquency**. Every individual in this high-risk group has already demonstrated a history of failing to meet their financial obligations, making this the single most reliable behavioral predictor of future trouble.

2.  **Exhausted Financial Flexibility (High CUR):** These borrowers are living on the edge of their available credit. With an average **Credit Utilization Rate (CUR) of 70%**, they have almost no financial buffer to absorb unexpected expenses, forcing them to prioritize payments and making them vulnerable to a cascading default.

3.  **Unsustainable Debt Burden (High DTI):** A significant portion of their income is already consumed by existing debt before accounting for their Nova Bank loan. An average **Debt-to-Income (DTI) ratio of 43%** indicates that their financial obligations are becoming unmanageable relative to their earnings.

4.  **Overleveraged Loan Size (High LTI):** The loan from Nova Bank itself contributes significantly to their financial pressure. With an average **Loan-to-Income (LTI) ratio of 40%**, the loan payment represents a substantial portion of their annual income, adding to their already strained budget.

## **Recommendations**

Based on the comprehensive analysis of borrower profiles, loan characteristics, and early warning indicators, we recommend Nova Bank implement a three-pronged strategic approach to fundamentally strengthen its credit risk framework. These actions are designed to reduce financial losses, enhance portfolio quality, and foster more responsible and sustainable lending practices.

#### **1. Strategic Overhaul of Underwriting and Risk Assessment**

The most immediate priority is to tighten the criteria for new loan origination to prevent high-risk assets from entering the portfolio.

*   **Immediately Revise Loan Grade Standards:**
    *   **Cease Origination:** Halt all new lending for loans graded **F and G**, as their near-100% loss rates make them financially unviable.
    *   **Intensive Scrutiny:** Place all applications for **Grade D and E** loans under the highest level of review, with a strong bias toward rejection unless significant mitigating factors are present.

*   **Enforce Strict Affordability Thresholds:**
    *   **Implement a Hard LTI Cap:** Automatically reject or subject applications with a **Loan-to-Income (LTI) ratio exceeding 0.4** to a mandatory senior underwriter review. The data clearly shows this is the point where default risk becomes unmanageable.
    *   **Scrutinize Debt-to-Income (DTI):** Pay special attention to applicants with high DTI ratios, particularly those in lower income brackets.

*   **Prioritize Proven Risk Indicators:**
    *   **Elevate Home Ownership Status:** Use home ownership as a primary differentiating factor in risk assessment. Apply more conservative terms (e.g., lower loan amounts, higher required income) for non-homeowners.
    *   **Penalize Past Delinquencies:** Integrate the number of past delinquencies directly into the risk score. Applications with a history of two or more delinquencies should automatically trigger enhanced due diligence.

*   **Shift Focus from Employment Type to Income Verification:**
    *   De-emphasize employment status (e.g., full-time vs. self-employed) as a primary risk factor and redirect resources toward robust income verification and cash flow analysis.

#### **2. Implement a Proactive Portfolio Management and Intervention Program**

For the risk already present in the portfolio, the bank must shift from a reactive to a proactive stance.

*   **Launch an Immediate Intervention Program:**
    *   Target the **122 accounts identified by the Early Warning Indicators** for immediate outreach.
    *   Employ a supportive, tiered communication strategy, beginning with offers of financial counseling and voluntary account reviews.
    *   Be prepared to offer tailored solutions like **payment restructuring** or **debt consolidation** to help at-risk customers avoid default.

*   **Establish a "High-Risk Watch List":**
    *   In addition to the 122 flagged accounts, place all existing loans graded **D and E** on a formal watch list for heightened monitoring and potential proactive engagement.

#### **3. Refine Pricing Models and Product Strategy**

Finally, a longer-term strategic review of pricing and product offerings is needed to ensure they align with the bank's risk appetite.

*   **Re-evaluate the High-Interest Rate Strategy:**
    *   For segments with extremely high default rates (e.g., 85% for rates >20%), the goal should be to **avoid originating these loans**, not merely to price them higher. The current interest premium is insufficient to cover the near-certain losses.

*   **Conduct a Targeted Analysis of Loan Products:**
    *   Investigate the anomaly driving higher default rates for **24-month loan terms**.
    *   Differentiate underwriting processes based on **loan purpose**, applying stricter reviews for higher-risk categories like Debt Consolidation and Medical loans.

By implementing these recommendations, Nova Bank can significantly reduce its loss rate, improve the overall health of its loan portfolio, and build a more resilient, profitable, and responsible lending institution.
