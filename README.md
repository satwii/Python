# Project Title: Stochastic Optimization and Feature Selection

## Description
This project integrates stochastic optimization algorithms and image processing techniques for two distinct tasks:

1. **Stochastic Hill Climbing for Puzzle Reassembly**:
   - Splits an image into grid pieces.
   - Reassembles the image by minimizing edge mismatches between adjacent pieces.
   - Implements the hill climbing algorithm with restarts to optimize the puzzle configuration.

2. **Stochastic Feature Selection for Recipe Recommendation**:
   - Fetches recipes based on user-provided ingredients and dietary restrictions.
   - Uses a stochastic feature selection approach to recommend recipes that best match user preferences.

## Features
### Puzzle Reassembly
- **Image Splitting**: Divides an image into equal grid pieces.
- **Mismatch Calculation**: Evaluates pixel mismatches along edges between pieces.
- **Hill Climbing Algorithm**: Optimizes the puzzle arrangement to minimize total mismatch.
- **Visualization**: Displays the puzzle during and after reassembly.

### Recipe Recommendation
- **Ingredient-Based Search**: Finds recipes matching user-provided ingredients using the Spoonacular API.
- **Dietary Restrictions**: Accounts for preferences such as vegan or gluten-free.
- **Stochastic Feature Selection**: Randomly samples subsets of recipes to optimize recommendations.

## Technologies Used
- **Programming Languages**: Python
- **Libraries**:
  - `PIL` (Pillow) for image processing
  - `numpy` for numerical computations
  - `matplotlib` for visualization
  - `requests` for API interactions
- **APIs**:
  - Spoonacular API for recipe data

## Installation
### Prerequisites
- Python 3.8 or higher
- Required Python libraries: Install using the command:
  ```bash
  pip install -r requirements.txt
  ```

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/stochastic-optimization.git
   ```
2. Set up the Spoonacular API key:
   - Obtain an API key from [Spoonacular](https://spoonacular.com/food-api).
   - Replace the placeholder in the code:
     ```python
     API_KEY = 'your_api_key_here'
     ```
3. Run the project:
   ```bash
   python main.py
   ```

## How to Use
### Puzzle Reassembly
1. Place image files (e.g., `samosa.jpg`) in the project directory.
2. Update the `main` function with the image file paths.
3. Run the script to visualize and reassemble the images.

### Recipe Recommendation
1. Update the `main` function with your ingredients and dietary restrictions.
2. Run the script to fetch and display recommended recipes.

## Example Output
### Puzzle Reassembly
- Displays the puzzle grid before and after reassembly.
- Shows the reassembled image.

### Recipe Recommendation
- Lists the top recipe recommendations based on user preferences.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Description of your changes"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Create a pull request.

