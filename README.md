
Claude finished the response
1788507668710_image.png
1788507696473_image.png
1788507711259_image.png
عايز بداية تكون زي كده شوف الاحسن واعمله

Ran 2 commands
Great palette reference. Let me extract precise colors and rebuild the whole deck in this style.

Ran a command, created a file
كمل

Ran 3 commands, read a file
This is looking very close to the reference style. Let's check the rest.

Read a file, ran a command, shared files
عملت البرزنتيشن كله بالتصميم الجديد ده (مش بس البداية) عشان يبقى فيه اتساق بصري من أول سلايد لآخر واحد:

استخدمت نفس الباليت بالظبط اللي طلعتها من الصور اللي بعتها: كحلي 
#2B2D42 وأحمر 
#EF233C.

البنية الجديدة (18 سلايد):

Title — نفس الستايل بتاعك بالظبط (دائرة حمرا، badge الصفحة، إلخ)
Agenda — 5 كروت (5 أقسام مطابقة لمحتوى العرض بتاعنا)
Project Objective — بانل كحلي جانبي + دايرة حمرا + 4 نقاط
Dataset Overview — 4 stat cards + كارت المجموعات الأربعة للأعمدة
Data Cleaning & Quality Checks — 4 كروت (missing/type/duplicate/outlier)
Summary Statistics — جدول + كارت insight
Executive Snapshot — الـ KPIs الرئيسية
8-17. الأسئلة العشرة — نفس المحتوى والرسومات بتاعتنا، بس بالباليت الجديد (وحتى شارتات الـ heatmap والـ yearly trend اتعملهم recolor يتماشوا مع نفس الألوان)
Conclusions — التوصيات النهائية
كل سلايد فيها نفس الـ footer وبادچ رقم الصفحة واللوجو زي اللي في الصور المرجعية بتاعتك.


Car sales business questions
Presentation·PPTX 
1788523402681_image.png
ظبط لون دي

تحديد سبب ظهور الرقم والنسبة معًا في التسمية.
Found it — the pie chart was showing both the raw value and the percentage stacked together (47.4 + 47%), and the label color was dark navy text sitting on a red/navy slice, so it's barely readable. Let me fix both.

Ran 4 commands, edited a file, and 2 more tools
لقيت المشكلة: الشارت كان بيعرض الرقم الخام (47.4) والنسبة المئوية (47%) مع بعض فوق بعض على نفس القطعة، وده اللي كان شكله مبعثر وملخبط. عدّلتها تعرض النسبة بس (47% / 53%) بخط أبيض واضح يبان كويس على الأحمر والكحلي. الملف اتحدّث.


Car sales business questions
Presentation·PPTX 
عايز [README.md](https://github.com/Ismail-Mahmoud-Mohamed/Car_Sales/commit/d59af6404662cea0e4ac93e82e6ed4a3160f2952#diff-b335630551682c19a781afebcf4d07bf978fb1f8ac04c6bf87428ed5106870f5)

Read a page, ran a command, and 2 more tools
شفت الريبو بتاعك على GitHub — لسه فيه README.md فاضي بس فيه # Car_Sales. عملتلك README.md كامل يوثّق المشروع كله (Phase 1 + Phase 2، الداتا، الـ 10 أسئلة، أهم النتائج، هيكل الملفات، وطريقة التشغيل)، جاهز تحطه في الريبو بدل الملف الحالي.


Readme
Document·MD 

Write a message…


Claude is AI and can make mistakes. Please double-check responses.


Readme · MD
🚗 Car Sales Data Analysis
An end-to-end exploratory data analysis (EDA) of a two-year, dealership-level car sales dataset — built to answer the ten business questions a dealership owner needs to make decisions on inventory, pricing, and regional investment.

📌 Project Overview
Each row in the dataset represents one completed car sale transaction: who bought it, what dealer sold it, which vehicle it was, and at what price. This project walks through two phases:

Phase 1 — Dataset Understanding & Profiling: business context, data dictionary, data types, missing values, duplicates, cardinality, and a full statistical profile of every column.
Phase 2 — Cleaning & Exploratory Data Analysis: light cleaning, outlier screening, KPI overview, distributions, correlation analysis, segment analysis, and the 10 key business questions — each with a chart and a plain-language, decision-ready takeaway.
📊 Dataset
Rows	23,906 transactions
Columns	16 attributes
Date range	2022 – 2023
Grain	One row = one car sale
Column groups:

Group	Columns
Transaction	Car_id, Date
Customer	Customer Name, Gender, Annual Income
Vehicle	Company, Model, Engine, Transmission, Color, Body Style, Price ($)
Dealer	Dealer_Name, Dealer_No, Dealer_Region, Phone
🎯 Project Objective
Identify the best-selling companies, models, and body styles.
Compare average pricing across segments and regions.
Track how monthly sales evolve over the two-year period (seasonality).
Explore whether customer income relates to the price of the car purchased.
🧹 Data Cleaning & Quality Checks
Check	Result
Missing values	1 row missing Customer Name was dropped (23,906 → 23,905 rows); every other column was fully complete
Type conversion	Date parsed to datetime; categorical columns cast accordingly
Duplicate rows	0 exact duplicates found — no de-duplication needed
Outlier scan (IQR)	Annual Income and Price ($) are both right-skewed, with high-end outliers consistent with luxury purchases
🔟 The 10 Business Questions
Which car companies (brands) sell the most units?
Which car models are most popular?
Which body style dominates sales?
Automatic vs Manual — what's the real split?
Which dealer regions generate the most sales?
Which body style commands the highest average price?
Which company has the highest average price?
Is there a relationship between customer income and car price?
How do sales change over time (seasonality)?
Which companies generate the highest total revenue?
Headline findings
Total revenue: $671.5M · Average price: $28,090 · Median price: $23,000
Top brand by units & revenue: Chevrolet (1,819 units / $47.7M)
Dominant body style: SUV (6,374 units) — but Sedans carry the highest average price
Transmission split: 52.6% Automatic / 47.4% Manual — closer than most assume
Top regions: Austin and Janesville lead the dealer network
Income vs. price correlation: ≈ 0.01 — essentially no linear relationship
Seasonality: both 2022 and 2023 follow the same pattern — slow start (Jan–Feb), a peak in September, a dip in October, and the strongest months in November–December
🗂️ Repository Structure
Car_Sales/
├── Cars_Analysis.ipynb                     # Full notebook: Phase 1 (Profiling) + Phase 2 (Cleaning + EDA)
├── car_data.csv                            # Source dataset (23,906 rows × 16 columns)
├── Car_Sales_Business_Questions.pptx       # Stakeholder-ready presentation of the 10 questions
└── README.md
🛠️ Tools
Python · Pandas · NumPy · Matplotlib · SciPy

▶️ How to Run
bash
git clone https://github.com/Ismail-Mahmoud-Mohamed/Car_Sales.git
cd Car_Sales
pip install pandas numpy matplotlib scipy jupyter
jupyter notebook Cars_Analysis.ipynb
✅ Recommendations
Protect top sellers — keep Chevrolet, Dodge, Ford, and the SUV/Hatchback body styles always in stock.
Budget by revenue, not units — a brand's revenue rank can outpace its unit rank (e.g. Oldsmobile); weight marketing spend accordingly.
Expand where demand already is — Austin and Janesville are proven regions for new outlets or added floor space.
Upsell through Sedans & premium brands — Sedans and Cadillac/Saab/Lexus carry the highest average prices; target financing offers there.
Plan for seasonality — monthly sales swing more than 6x; align staffing and promotions with the stronger months.
Don't assume income drives price choice — income and price are essentially uncorrelated; build strategy on behavior, not income alone.
⚠️ Limitations
This is observational sales data with no causal proof behind any pattern; regional and dealer imbalance may confound simple rankings. Gender and Annual Income are sensitive fields and are used here for descriptive/audit purposes only — never for differential pricing or targeting.

Graduation Project — Exploratory Data Analysis




