1. Open PowerBI Desktop using the given Excel Data file.
2. Create Visualizations:  
    a. Create a combination of line and bar charts to compare actual revenue and expenses against budgeted figures.

   - Click on **Line** and **Stacked Column Chart** from the **Visualizations Pane** (first one shown in the picture under Vocabulary heading above), and place it on the Page.
   - Drag **Actual Expenses** from **Data Pane** to the **Visualizations Pane** under **Line y-axis**. Drag **Budgeted Expenses** from the **Data Pane** to the **Visualizations Pane** under **Column y-axis**.
   - Drag **Date** from the **Data Pane** to the **Visualizations Pane** under **X-axis**.
   - You may remove unnecessary indications such as **Quarter** and **Day** from the **X-axis** metric under the **Visualizations Pane**.
   - Follow the same Procedure from Step 3 to 5 for **Actual Revenue** and **Budgeted Revenue**. This would result in two combined **Line and Bar Charts** comparing **A**ctual and **Budgeted figures** for **Expenses** and **Revenue**.

     b. Use a gauge chart to display key financial metrics such as net profit margin.

   - To use **Net Profit Margin** in our reports, we need Columns such as **Profit** and **Net Profit Margin**.

   Profit \= Actual Revenue \- Actual Expenses

   Net Profit Margin (%) \= ProfitActual Revenue 100

   - Navigate to **Table View**. Click on any of the Columns in your table, and click on the **New Column** option that appears on top.
   - Clear the **formula input** (the input bar in the above picture with ‘`Column =`’ in it) and type in the following: (Here, financial is the name of the Data File you are using)

   `Profit = financial[Actual Expenses] - financial[Actual Revenue]`

   - Follow the same procedure to add a column called **Net Profit Margin** to the Data. Use the formula: (Here, financial is the name of the Data File you are using)

   `Net Profit Margin = (financial[Profit] / financial[Actual Revenue]) * 100`

   - Now go back to the default **Report View** where your charts are located. Use the **Page Pane** to create a new Page.
   - Click on **Gauge Chart** from the **Visualizations Pane** (third one shown in the picture under Vocabulary heading above), and place it on the new Page.
   - Now, click on the **New Measure** option appearing on the **Top Bar**. This Option allows you to use figures in your visualizations without having to create new Columns.
   - In the **Input Field** that appears, enter `MaxValue = 100`. This creates a new measure in your columns, called **MaxValue**, that you can use.
   - Follow the same to create two other values: `MinValue = 0` and `TargetValue = 35`.
   - Now, click on the **Gauge Chart** in your page to activate the **Visualizations Pane**. From the **Data Pane,** drag **Net Profit Margin** to the **Value Field** in the **Visualizations Pane**. Click on the **Net Profit Margin** that was just dragged, and click **Average**, instead of **Sum**. This would let us create the **Gauge Chart** with the average of the **Net Profit Margin** values in the Column.
   - Now drag **MaxValue** from the **Data Pane** to the **Maximum Value** field in the **Visualizations Pane**. Similarly, drag the **MinValue** from the **Data Pane** to the **Minimum Value** field and the **TargetValue** from the **Data Pane** to the **Target Field**.

     c. Create a waterfall chart to show the contribution of different factors to the overall profit.

   - Use the **Page Pane** to create a new Page.
   - Click on **Waterfall Chart** from the **Visualizations Pane** (second one shown in the picture under Vocabulary heading above), and place it on the new Page.
   - From the **Data Pane**, drag **Category** to the **Category Field** in the **Visualizations Pane**.
   - Drag **Profit** from the **Data Pane** to the **Y-axis** field in the **Visualizations Pane**.
   - Drag any one of the values: **Budgeted Expenses**, **Budgeted Revenue**, **Actual Expenses** or **Actual Revenue** to the **Breakdown Field** in the **Visualizations Pane**. This would give you the **Waterfall Chart** corresponding to the effect of the chosen field on the **Profit** value based on product **Category**.

3. Your multi-page dashboard/report is now ready. You may save it for future use.
