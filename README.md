# First Submission: Solving Human Resource Problem
## Business Understanding
Jaya Jaya Maju, a multinational company established in 2000 with over 1,000 employees across Indonesia, is facing a significant challenge with its employee attrition rate exceeding 10%. This high turnover suggests potential issues with job satisfaction, career management, compensation, or overall working conditions, leading to financial and productivity losses.

To address this, the HR department requires a data-driven dashboard to monitor and analyze the factors causing high attrition. This tool will help them visualize current trends and take corrective action. Additionally, they need a machine learning model to predict which employees are likely to leave.

### Business Problems
> 📊 Business Problem 1: **How is the relationship between the variables or factors from the available data and employee attrition?**

🔍 It's important to understand how different things about employees and their jobs connect to whether they leave the company. By seeing these connections, the company can get a clearer picture of what might make someone stay or go, which helps in making smarter decisions to keep their workforce happy and stable.

> 🛠️ Business Problem 2: **What are the recommended actions that companies can take to prevent employee attrition?**

✅ Knowing what steps to take helps companies keep their good workers happy and wanting to stay. This saves the company money and trouble because they don't have to keep finding and training new people all the time.

> 🔮 Business Problem 3: **How to predict the risk of employee attrition before employees actually leave the company?**

🚨 If the company can get an early warning that someone might be thinking of leaving, they can talk to that employee and try to fix any issues. This gives them a chance to keep good people from walking out the door.

### Project Scope

## Business Dashboard
Dashboard for this project was developed using Looker Studio. It can be seen in this [Link](https://lookerstudio.google.com/reporting/1c83537d-9f4f-473f-b7a1-0e7dd37fd4d7) (login google account is required).

## Conclusion (based on the Dashboard)
### 📊 Business Problem 1: **How is the relationship between the variables or factors from the available data and employee attrition?**
The analysis reveals that **employee attrition is driven by a combination of job conditions, personal satisfaction, career progression, and external factors**. These factors can be grouped into four major themes, each contributing uniquely to an employee’s decision to stay or leave.

---

1. 🧱 **Job Demands & Role**
**Key Variables**: `OverTime`, `JobRole`, `BusinessTravel`

- Employees working **overtime** or in roles requiring **frequent travel** face higher stress and burnout, leading to increased attrition.
- Specific roles like **Sales Representative** show disproportionately high turnover, indicating that **attrition is concentrated in certain positions**, not evenly spread across the company.

✅ **Takeaway**: High job demands and stressful roles are strong predictors of employee turnover.

---

2. 😊 **Employee Satisfaction & Engagement**
**Key Variables**: `JobSatisfaction`, `EnvironmentSatisfaction`, `JobInvolvement`, `WorkLifeBalance`

- **Low satisfaction** with the job or work environment is strongly associated with leaving.
- Employees who feel **disconnected or disengaged** in their roles are much more likely to quit.
- A **poor work-life balance** is a particularly strong indicator of potential attrition.

✅ **Takeaway**: Emotional and psychological connection to work is one of the most critical factors influencing attrition.

---

3. 📈 **Career History & Growth**
**Key Variables**: `TotalWorkingYears`, `NumCompaniesWorked`, `YearsSinceLastPromotion`, `TrainingTimesLastYear`

- **Early-career employees** (0–5 years of experience) are most likely to leave, often seeking growth.
- Both **low and high job mobility** are linked to higher attrition—moderate mobility suggests stability.
- Lack of **training opportunities** or career development support increases attrition.
- Interestingly, employees **recently promoted** also show high turnover, possibly due to shifting expectations or unmet promises.

✅ **Takeaway**: Employees leave when they feel stuck—or when they don’t see a clear, fulfilling path forward.

---

4. 💰 **Financial & External Factors**
**Key Variables**: `StockOptionLevel`, `DistanceFromHome`

- Employees without stock options feel **less financially invested** in staying.
- A **long commute** makes leaving more likely, likely due to lifestyle fatigue or lower quality of life.

✅ **Takeaway**: Incentives and daily life logistics significantly affect whether employees remain with a company.

---

📊 Overall Insight

There is **no single factor** that causes employee attrition. Instead, it results from **multiple interrelated elements** across work conditions, emotional satisfaction, personal development, and external life. Recognizing and addressing **key pain points**—like stressful roles, disengagement, lack of growth, and long commutes—can greatly reduce attrition and improve retention.

### 🛠️ Business Problem 2: **What are the recommended actions that companies can take to prevent employee attrition?**
Based on the analysis of employee data and attrition patterns, here are five actionable strategies companies can implement to reduce attrition, along with the key variables involved. These strategies are designed to be practical and easily understood:

---

1. **Implement Flexible Work & Remote Options**  
📌 **Key Variables:** `DistanceFromHome`, `WorkLifeBalance`, `OverTime`, `BusinessTravel`  
- **Why it matters:** Long commutes and poor work-life balance are common triggers of burnout, especially among those who travel frequently or work overtime.  
- **Action:** Offer hybrid or remote work options, flexible working hours, and clear policies on remote eligibility and expectations.

---

2. **Strengthen Career Pathing & Development Programs**  
📌 **Key Variables:** `YearsAtCompany`, `TrainingTimesLastYear`, `JobRole`, `PerformanceRating`  
- **Why it matters:** Employees—especially early in their careers—are more likely to leave if they don’t see clear growth paths or opportunities to upskill.  
- **Action:** Develop visible career ladders, mentorship programs, and increase access to meaningful training tied to promotions.

---

3. **Conduct "Deep Dive" Reviews into High-Stress Roles**  
📌 **Key Variables:** `JobRole`, `JobSatisfaction`, `OverTime`, `WorkLifeBalance`  
- **Why it matters:** Attrition often clusters around specific roles with heavy workloads or unique challenges, which standard policies may not address.  
- **Action:** Investigate high-turnover roles individually using focus groups and surveys to uncover root causes and implement tailored solutions.

---

4. **Enhance Support for Newly Promoted Employees**  
📌 **Key Variables:** `YearsSinceLastPromotion`, `JobSatisfaction`, `JobInvolvement`  
- **Why it matters:** Attrition tends to spike after promotions due to unclear expectations or insufficient support in new roles.  
- **Action:** Create structured onboarding plans post-promotion, including clear goals and regular check-ins to help employees succeed in their new responsibilities.

---

5. **Expand and Communicate Financial Incentives**  
📌 **Key Variables:** `StockOptionLevel`, `MonthlyIncome`, `TotalWorkingYears`  
- **Why it matters:** Employees without long-term financial incentives may feel less tied to the company and more open to outside offers.  
- **Action:** Expand stock option eligibility and communicate its value clearly. Provide financial wellness programs to help employees understand and appreciate their total compensation.

---

✅ Overall Recommendation:
To effectively reduce attrition, companies should adopt a **multi-pronged approach** that addresses both **personal employee needs** (flexibility, growth, support) and **structural incentives** (financial rewards, role-specific interventions). By focusing on the variables most closely linked to turnover, targeted and measurable actions can be taken to improve retention.

### 🔮 Business Problem 3: **How to predict the risk of employee attrition before employees actually leave the company?**
A predictive model has been developed to assess which employees are most at risk of leaving the company. This approach helps HR departments intervene **before** resignations occur, reducing unexpected turnover and supporting better workforce planning.

---

✅ Best Model Recommendation: **SMOTE + Logistic Regression**

📌 **Why this model is most effective:**
- **Balanced Performance**: Achieved the **highest F1-score (0.559)** while maintaining a good **recall (0.487)** and **accuracy (0.858)**.
- **Interpretable**: As a linear model, Logistic Regression makes it easy to understand which variables (e.g., `OverTime`, `JobSatisfaction`, `YearsAtCompany`) influence attrition risk.
- **Class Imbalance Solution**: SMOTE (Synthetic Minority Oversampling Technique) helps the model treat both attrition and non-attrition cases more fairly, avoiding bias toward the majority class.

---

📊 Key Variables That Predict Attrition Risk

These features were most influential in predicting if an employee might leave:
- `OverTime`: Frequent overtime is a strong indicator of burnout.
- `JobSatisfaction`: Low satisfaction scores correlate with higher attrition risk.
- `EnvironmentSatisfaction`: Poor perception of the workplace contributes to turnover.
- `YearsAtCompany`: Very short or very long tenure can signal flight risk.
- `StockOptionLevel`: Lack of financial incentives (e.g., no stock options) is a key driver.
- `TrainingTimesLastYear`: Limited training may reflect lack of development, increasing attrition risk.
- `DistanceFromHome`: Long commutes are associated with higher stress and attrition.

---

📈 How the Prediction System is Developed

1. **Clean & Prepare Data**: Categorical features like `JobRole` and `OverTime` are converted into machine-readable formats.
2. **Train the Model**: Models are trained on historical employee data to learn patterns associated with attrition.
3. **Use SMOTE**: Balances the number of attrition vs. non-attrition examples, so the model can learn from both.
4. **Predict Risk**: The model calculates an attrition risk score (e.g., 0 to 100%) for each current employee.
5. **Prioritize Interventions**: HR teams can focus retention efforts on those flagged with higher risk scores.

---

📌 Strategic Business Benefits

- **Early Warning System**: HR can proactively identify and support high-risk employees *before* they resign.
- **Cost Reduction**: Reduces expenses related to hiring, onboarding, and training new staff.
- **Data-Driven Decisions**: Model outputs help prioritize HR initiatives and guide personalized retention strategies.
- **Trust and Transparency**: Logistic Regression supports explainable decisions, improving adoption by HR and leadership.

---

🔄 Future Action Plan

- **Build a Dashboard**: Display employees ranked by attrition risk scores.
- **Automate Monthly Updates**: Keep predictions current with the latest HR data.
- **Retrain Periodically**: Update the model every 6–12 months to adapt to organizational changes.
- **Link to Action**: Combine predictions with programs like flexible work, training, and promotion support to prevent turnover.

---

🏁 Final Takeaway

The **SMOTE + Logistic Regression** model is the most practical and accurate tool to **predict employee attrition before it happens**. It transforms raw HR data into actionable insights, enabling smarter, earlier, and more effective employee retention strategies.
