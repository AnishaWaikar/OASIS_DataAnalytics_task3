# OASIS_DataAnalytics_task3
🏙️ Task 3 — Airbnb NYC Data Cleaning & Preparation

Objective

To clean and standardize the Airbnb NYC dataset so it can serve as a reliable foundation for downstream analysis. The primary goal was to convert inconsistent values into usable formats, handle missing and duplicate entries, and prepare the data for future modeling or exploratory analytics focused on pricing, occupancy, and property characteristics.

📝 Steps Performed

Data Import & Structural Review
Loaded the AB_NYC_2019.csv dataset and examined dimensions, column types, and previewed entries to assess data readiness.

Data Consistency Fixes
Converted Installs, Price, and Size equivalent values (where relevant) into numeric formats; standardized text-based fields for consistency across categories.

Critical Value Cleaning
Converted last_review to a timestamp for temporal analysis and imputed missing review frequency values (reviews_per_month = 0).
Dropped rows with missing Rating to avoid analytical distortion and removed duplicate records to prevent biased insights.

Outlier Handling (Price)
Detected extremes in price using the Interquartile Range (IQR) method and capped values to reduce skew — keeping realistic boundaries without discarding data.

Data Export & Validation
Reviewed the final dataset shape post-cleaning and exported to AB_NYC_2019_cleaned.csv for further report generation, visualization, or modeling tasks.

🛠 Tools Used

Python Libraries: Pandas, NumPy

Visualization: Matplotlib, Seaborn

Techniques: Missing-value handling, type conversions, duplicate removal, outlier treatment using IQR, string standardization

📌 Outcome

The dataset transitioned from raw and inconsistent to clean, structured, and analysis-ready. Price outliers were smoothed to preserve data integrity, textual inconsistencies were resolved, and timestamps were aligned to support time-based analysis. The cleaned dataset provides a dependable base for studying pricing trends, neighborhood patterns, host behavior, and relationships between property features and customer interest.
