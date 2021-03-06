﻿# Exercise 4: Optional exercise

**You can earn an additional +3 points with the completion of this exercise.** (In the evaluation, you will see the text "imsc" in the exercise title; this is meant for the Hungarian students. Please ignore that.)

The category system is currently hierarchical. We want to simplify this.

Write T-SQL code block that deletes every category that is not a top-level one (has non-empty `ParentCategoryId`) after moving all products from this category to the parent. Since the category system is a tree with multiple levels, you need to repeat this process as long as there are subcategories. You need to start from the bottom of the hierarch, and in each iteration, you need to handle the categories with parents, but are not parents themselves,

!!! example "SUBMISSION"
    Submit the code in file `f4.sql`. The file shall contain the T-SQL code. It should not include any `use` or `go` commands. The solution should be a single T-SQL code block. Do not use stored procedures or triggers here. (There is no need to delete the `ParentCategoryId` column.)

!!! example "SUBMISSION"
    Create a screenshot that shows the `Category` table after executing the script. Save the screenshot as `f4.png` and submit it with the other files of the solution. The screenshot shall display the database name (which should be your **Neptun code**) in the _Object Explorer_ window and the **contents of the `Category` table**. The screenshot is required to earn the points.
