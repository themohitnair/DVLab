### Steps for Creating the Financial Performance Dashboard:

1. **Import and Prepare Data**:

   - Open Tableau Public and click **Connect to a File** to upload your financial dataset.
   - Ensure the dataset includes columns for actual revenue, actual expenses, budgeted revenue, budgeted expenses, net profit, and date.

2. **Create Visualizations**:

   - **Line and Bar Chart (Actual vs. Budgeted Figures)**:

     - Drag `Date` (set to **Month**, **Quarter**, or **Year**) to **Columns**.
     - Drag `Actual Revenue`, `Budgeted Revenue`, `Actual Expenses`, and `Budgeted Expenses` to **Rows**.
     - Change the visualization type for revenue to a **Line Chart** and for expenses to a **Bar Chart**. Use dual-axis for better comparison and synchronize the axes.

   - **Gauge Chart (Net Profit Margin)**:

     - Create a calculated field for **Net Profit Margin**: `(Net Profit / Revenue) * 100`.
     - Use this field to create a **Gauge Chart** by customizing a circular chart and overlaying it with percentage metrics.

   - **Waterfall Chart (Profit Contribution)**:
     - Create a calculated field for factors contributing to overall profit (e.g., revenue streams, cost categories).
     - Drag these factors to **Columns** and their corresponding values to **Rows**.
     - Change the visualization type to **Waterfall Chart** by enabling running totals and adjusting color coding for positive and negative contributions.

3. **Design the Dashboard**:

   - Click **New Dashboard** and drag the visualizations onto the canvas.
   - Place the line and bar chart at the top for trend analysis, the gauge chart in the center for key metrics, and the waterfall chart at the bottom for detailed profit contribution.
   - Add **Filters** for time periods (e.g., monthly, quarterly, yearly) by dragging the `Date` field into the dashboard as a filter.
   - Include titles, legends, and tooltips for clarity and user interaction.

4. **Enhance Interactivity**:

   - Add **Action Filters** to allow users to click on specific areas of the dashboard to drill down into details.
   - Customize the layout to ensure responsiveness across different screen sizes.

5. **Publish and Share**:
   - Save the dashboard and publish it to Tableau Public for online access.
   - Share the link with stakeholders and ensure it’s interactive and user-friendly.
