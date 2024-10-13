# NodeJsAssignment

Target Calculator - Calculate Daily and Monthly Targets Excluding Fridays

Description:

This JavaScript class, TargetCalculator, helps you calculate daily and monthly working day targets based on a provided annual target, start date, and end date. It excludes Fridays from the calculation to provide a more accurate representation of working days.

Features:

Calculates working days: Excludes Fridays from the total number of days in a month.
Handles date ranges: Works with a specified start and end date range.
Calculates proportional targets: Distributes the annual target proportionally across working days within the range.
Provides monthly and total targets: Returns both individual monthly targets and the cumulative total target.
Installation:

This code snippet doesn't require any specific installation steps since it's vanilla JavaScript. You can copy and paste it directly into your project or use it as a reference for creating your own implementation.

Usage:

Create a TargetCalculator instance:

JavaScript
const calculator = new TargetCalculator('2024-01-01', '2024-03-31', 5220);
Use code with caution.

Replace '2024-01-01' with your desired start date (YYYY-MM-DD format).
Replace '2024-03-31' with your desired end date (YYYY-MM-DD format).
Replace 5220 with your annual target value.
Run the calculation:

JavaScript
const results = calculator.run();
Use code with caution.

This will call the run method and return an object containing the following properties:

totalDaysExcludingFridays: An array containing the total number of working days (excluding Fridays) in each month within the date range.
actualWorkedDays: An array containing the actual number of working days you worked in each month (excluding Fridays).
monthlyTargets: An array containing the calculated daily target for each working day in each month (proportional to the annual target).
totalTarget: The cumulative total target for the entire date range.
Access the results:

console.log(results); // This will print the calculated values

Example Output:

{
  totalDaysExcludingFridays: [21, 20, 22], // Assuming no holidays in this example
  actualWorkedDays: [/* Your actual worked days here */],
  monthlyTargets: [/* Your daily targets for each month here */],
  totalTarget: /* Your total target for the period here */
}



Additional Notes:

You can modify the code to include weekends or specific holidays in the calculation by adjusting the logic in the calculateDays function.
Consider adding error handling for invalid date inputs.
For more complex scenarios, you might want to create a library with additional features like target tracking, reporting, and persistence.
