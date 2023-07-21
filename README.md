function findMaximum(numbers) {
  if (!Array.isArray(numbers) || numbers.length === 0) {
    return undefined; // Return undefined for invalid inputs or empty arrays
  }

  let maximum = numbers[0]; // Assume the first number is the maximum

  for (let i = 1; i < numbers.length; i++) {
    if (numbers[i] > maximum) {
      maximum = numbers[i]; // Update maximum if a larger number is found
    }
  }

  return maximum;
}
