# PL-900 - Lab 1 - Data Modeling
v9.6

## Scenario

Bellows College is an educational organization with multiple campuses and programs. Many of Bellow Colleges instructors and administrators need to attend events, and purchase items. Historically tracking these expenses has been a challenge. 

Campus administration would like to modernize their expense reporting system by providing employees with a digital way to report expenses. 

Throughout this course, you will build applications and perform automation to enable the Bellows College employees to manage expenses.

## High-level lab steps

- Create the Expense Report table
- Create columns in the table
- Add some sample data. 

## Prerequisites

- Completion of **Lab 0 - Validate lab environment**

## Exercise 1: Create New Table and Columns

**Objective:** In this exercise, you will create a new custom table for Expense Reports and add appropriate columns.

### Task #1: Create Expense Report Table

The **Expense Report** table will contain information about individual expenses that an employee can submit including reason, type, date, and amount.

1. If you are not already signed in, sign into https://make.powerapps.com

1. From the **Environment** menu in the top right, ensure the **Dev One** environment is selected.

1. Using the navigation on the left, select **Tables**.

1. Select **+ New table** and choose **Set advanced properties**.

1. For **Display name**, enter **Expense Report**.

1. Select **Save**.

1. Under the **Schema** section, select **Columns**.

### Task #2: Create Columns
#### 1. Create Expense Date Column
- Create a column named **Expense Date** that is type **Date Only**
- Set it to **Business Required**.
- Also set the the **Time Zone Adjustment** as **Date Only**.


<details>
<summary>Click here to expand these instructions if you need step-by-step guidance.</summary>

<ol>

<li>Select <b>+ New column</b>.</li>
<li>Enter <b>Expense Date</b> for <b>Display name</b>.</li>
<li>Select <b>Date only</b> for <b>Data type</b>.</li>
<li>Change <b>Required</b> to <b>Business required</b>.</li>
<li>Expand <b>Advanced options</b>.</li>
<li>In <b>Time zone adjustment</b>, select <b>Date Only</b>.</li>
</ol>

<b>Note:</b> We use <b>Date only</b> behavior to record date information, because the date of the Expense Report should not change when viewed from a different time zone.

7. Select <b>Save.</b>
</details>


1. #### Create Expense Type Column

	1. Select **+ New column**.

	1. Enter Expense Type for **Display name**.

	1. Select **Choice** for **Data type**.

	1. In **Required**, select **Optional**.

	1. Set **Sync with global Choice** to **Yes (recommended)**

	1. In **Sync this choice with** field, select **Expense Type**.

	1. Set the **Default choice** field to **None**.

	1. Select **Save**.

1. #### Create Expense Purpose Column

	1. Select **+ New column**.

	1. Enter Expense Purpose for **Display name**.

	1. Select **Choice** for **Data type**.

	1. In **Required**, select **Optional**.

	1. Set **Sync with global Choice** to **Yes (recommended)**

	1. In **Sync this choice with** field, select **Expense Purpose**.

	1. Set the **Default** field to **None**.

	1. Select **Save**.

1. #### Create Item Description column

	1. Select **+ New column**.

	1. Enter Item Description for **Display name**.

	1. Select **Multiple Lines of text &gt; Plain Text** for **Data type**.

	1. Select **Save**.

1.  #### Create Expense Amount column

	1. Select **+ New column**.

	1. Enter Expense Amount for **Display name**.

	1. Select **Currency** for **Data type**.

	1. Select **Save**.

 
## Exercise 2: Enter data

**Objective:** In this exercise, you manually enter some sample data into your new table. 

### Task #1: Modify the columns displayed

1. Open the **Expense Report** table.

1. Next to the **Name** column, select **+26 more**.

1. From the menu that appears, select the following columns:

	1. Expense Date

	1. Expense Purpose 

	1. Expense Type

	1. Expense Amount

	1. Item Description

1. Select the **Save** button.

### Task #2: Add a sample record.

1. Select the **Arrow** next to **Edit**. From the menu that appears, select **Edit in new tab**.

1. In the **Name** column, enter **John Doe**.

1. In the **Expense Date** column, enter **xxx**.

1. In the **Expense Purpose**, select **Conference**.

1. In the **Expense Type** column, select **Travel**.

1. In the **Expense Amount** column, enter **750.00**.

1. In the **Item Description**, enter a short description.

1. Hit the Tab button to advance to the next row and **save** the record.

Congratulations, you have successfully created a new table and added data.

