# Binary Search Visualization

An interactive tool to help you understand the **Binary Search** algorithm.

**Access the Visualizer**: Click [here](https://3disturbed.github.io/BinarySearchVisual/BinarySearchVisualizer.html) to open the Binary Search Visualizer in your web browser.

![Binary Search Visualization](https://github.com/user-attachments/assets/098bf2fb-0658-4410-a4fd-11164e260bd5)

**Access the Visualizer**: Click [here](https://3disturbed.github.io/BinarySearchVisual/BinarySearchVisualizer.html) to open the Binary Search Visualizer in your web browser.

## Introduction

Binary Search is a fundamental algorithm used to efficiently find a target value within a **sorted** array. By repeatedly dividing the search interval in half, it quickly narrows down the possible locations of the target value, making it much faster than a linear search, especially for large datasets.

This visualization tool provides a step-by-step graphical representation of the Binary Search algorithm, allowing you to interactively see how it works internally.

## Features

- **Interactive Visualization**: Watch how the search interval narrows down with each step.
- **Custom Input**: Enter your own sorted arrays and target values to see how the algorithm performs.
- **Step-by-Step Execution**: Control the speed of the visualization to better understand each operation.
- **Educational**: Great for students and anyone interested in learning how Binary Search works.

## How to Use the Visualizer

1. **Access the Visualizer**: Click [here](https://3disturbed.github.io/BinarySearchVisual/BinarySearchVisualizer.html) to open the Binary Search Visualizer in your web browser.
2. **Input Data**:
   - **Array**: Enter a sorted array of numbers separated by commas (e.g., `1, 3, 5, 7, 9`).
   - **Target Value**: Enter the number you want to search for in the array.
3. **Start Visualization**: Click the **"Start"** button to begin the visualization.
4. **Control Execution**:
   - Use the **"Pause"** and **"Resume"** buttons to control the flow.
   - Adjust the speed slider to slow down or speed up the visualization.
5. **Observe**: Watch as the algorithm highlights the middle element and adjusts the search boundaries (`low`, `mid`, `high`) in each step.

## Understanding Binary Search

Binary Search works on the principle of divide and conquer. Here's a brief overview:

1. **Initialize**:
   - Set `low` to the first index of the array.
   - Set `high` to the last index of the array.
2. **Loop**:
   - While `low` is less than or equal to `high`:
     - Calculate `mid` as the floor of `(low + high) / 2`.
     - If the element at `mid` is equal to the target, the search is successful.
     - If the target is less than the element at `mid`, set `high = mid - 1`.
     - If the target is greater than the element at `mid`, set `low = mid + 1`.
3. **Result**:
   - If the target is found, return its index.
   - If the target is not found, indicate that it does not exist in the array.

### Time Complexity

- **Best Case**: O(1) when the middle element is the target.
- **Average and Worst Case**: O(log n), making it highly efficient for large datasets.

## Applications

- **Databases**: Quickly searching for records.
- **Libraries**: Looking up books or resources.
- **Gaming**: Collision detection and resource management.
- **Networking**: Routing and IP address management.

## Example

Suppose you have the sorted array `[2, 4, 6, 8, 10, 12, 14]` and you want to find the target value `10`.

- **Step 1**:
  - `low = 0`, `high = 6`, `mid = 3`.
  - Element at `mid` is `8`.
- **Step 2**:
  - `10 > 8`, so set `low = mid + 1 = 4`.
- **Step 3**:
  - `low = 4`, `high = 6`, `mid = 5`.
  - Element at `mid` is `12`.
- **Step 4**:
  - `10 < 12`, so set `high = mid - 1 = 4`.
- **Step 5**:
  - `low = 4`, `high = 4`, `mid = 4`.
  - Element at `mid` is `10`.
- **Result**:
  - Target found at index `4`.

## Contribute

Contributions are welcome! If you have suggestions for improvements or find any bugs, feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- Inspired by the need to make learning algorithms more interactive and engaging.
- Thanks to all the contributors who have helped improve this project.

---

**Use the Visualizer Now**: [Binary Search Visualizer](https://3disturbed.github.io/BinarySearchVisual/BinarySearchVisualizer.html)
