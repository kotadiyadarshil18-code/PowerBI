📊 Sales Data Model – Power BI Project
📌 Project Overview

This project focuses on Data Modeling & Relationships in Power BI using a Star Schema approach.

No heavy visualization focus ❌
Focus on data modeling, relationships & optimization ✅

🖼️ Step-by-Step Presentation
🔹 Step 1: Project Introduction

Project Title: Sales Data Model
Tool Used: Power BI
Objective:

Build a Star Schema Data Model
Define relationships (PK–FK)
Optimize model for analysis
🔹 Step 2: Data Loading (Power Query)

Tasks:

Import all Excel files:
Sales_Fact
Customer_Dim
Product_Dim
Region_Dim
Date_Dim
Returns_Fact
Apply:
Correct data types
Remove blank rows
Clean unnecessary columns
🔹 Step 3: Table Structure Understanding

Fact Tables:

Sales_Fact
Returns_Fact

Dimension Tables:

Customer_Dim
Product_Dim
Region_Dim
Date_Dim
🔹 Step 4: Relationships Creation

Create relationships:

Sales_Fact → Customer_Dim
Sales_Fact → Product_Dim
Sales_Fact → Region_Dim
Sales_Fact → Date_Dim
Returns_Fact → Sales_Fact
Returns_Fact → Date_Dim (Inactive relationship)
🔹 Step 5: Keys Definition

Primary Keys (PK):

CustomerID
ProductID
RegionID
DateKey
SalesID

Foreign Keys (FK):

CustomerID (in Sales_Fact)
ProductID (in Sales_Fact)
RegionID (in Sales_Fact)
DateKey (in Sales_Fact & Returns_Fact)
🔹 Step 6: Schema Design

Model Type: Star Schema ⭐

Structure:

Central Table → Sales_Fact
Connected Dimensions → All Dim Tables

Additional:

Returns_Fact as:
Secondary Fact Table OR
Snowflake extension
🔹 Step 7: Relationship Cardinality

Used Types:

One-to-Many (1:*) → Most relationships
Many-to-One (*:1) → Fact → Dimension
One-to-One (1:1) → Rare cases
🔹 Step 8: Cross Filter Direction

Rules Applied:

Default → Single Direction ✅
Bidirectional → Only when required ⚠️
🔹 Step 9: Advanced Model Settings

Tasks:

Enable / Disable Bidirectional Filters
Handle inactive relationship (Returns Date)
Resolve filter ambiguity issues
🔹 Step 10: Data Formatting

Set Formats:

Revenue → Currency 💰
Quantity → Whole Number
Date → Date format
🔹 Step 11: Data Categories

Apply categories for better visuals:

City → City
Country → Country
ProductName → Product
🔹 Step 12: Hierarchies Creation

Created Hierarchies:

📅 Date_Dim:
Year → Quarter → Month → Date

🌍 Region_Dim:
Country → State → City

📦 Product_Dim:
Category → Subcategory → ProductName

🔹 Step 13: Model Validation

Check:

Relationships working correctly ✅
No ambiguity ❌
Filters behaving properly ✅
🔹 Final Output

✅ Star Schema Data Model Created
✅ Relationships Optimized
✅ Ready for Reporting & DAX


<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/c9c1d441-e2c5-498b-b139-6e94549632a9" />
