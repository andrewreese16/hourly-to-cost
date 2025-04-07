// Function to calculate hours
function calculateHours() {
  // Get values from input fields
  let wage = parseFloat(document.getElementById("wage").value);
  let itemCost = parseFloat(document.getElementById("item-cost").value);

  // Check if inputs are valid numbers
  if (isNaN(wage) || isNaN(itemCost) || wage <= 0 || itemCost <= 0) {
    alert("Please enter valid numbers for both hourly wage and item cost.");
    return;
  }

  // Calculate the number of hours
  let hoursToWork = itemCost / wage;

  // Display the result
  document.getElementById(
    "hours-to-work"
  ).innerText = `It would take you ${hoursToWork.toFixed(
    2
  )} hours to purchase this item.`;
}

// Add event listener to detect Enter key press
document.getElementById("wage").addEventListener("keydown", function (event) {
  if (event.key === "Enter") {
    document.getElementById("item-cost").focus(); // Move to next input
  }
});

document
  .getElementById("item-cost")
  .addEventListener("keydown", function (event) {
    if (event.key === "Enter") {
      calculateHours(); // Calculate after Enter key is pressed in the second field
    }
  });
