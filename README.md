

# 🎨 Python Data Visualization Programs

![Data Visualization Banner](/api/placeholder/800/200)

This repository contains Python programs focused on **data visualization** and related logic, along with **program documentation** and **viva questions** to help understand key concepts.

---

## 📊 Program 1: Best Test Average and Palindrome Number 🔢

<details>
<summary><h3>Working</h3></summary>

- Accepts three test marks, removes the lowest score, and calculates the average of the best two.
- Checks if a number is a palindrome using string reversal.
- Counts occurrences of each digit in the number.
</details>

<details>
<summary><h3>Viva Q&A</h3></summary>

**Q1: How does the `min()` function help in finding the best two scores?**  
> It identifies the lowest score among three test marks, which is subtracted from the total to find the sum of the best two scores.

**Q2: What happens with non-numeric input?**  
> A `ValueError` is raised. A `try-except` block handles the exception by displaying an error message.

**Q3: Explain `number[::-1]` in palindrome checking.**  
> String slicing with `[::-1]` reverses the string. The `[::-1]` syntax denotes start:end:step where a `-1` step traverses backward.

**Q4: How does the digit-counting dictionary work?**  
> The program creates an empty dictionary, iterates through each character, checks if it’s a digit using `isdigit()`. If the digit exists as a key, it increments its count; otherwise, it adds a new key with a count of 1.
</details>

---

## 📊 Program 2: Fibonacci and Number Conversions 🔄

<details>
<summary><h3>Working</h3></summary>

- Implements the Fibonacci sequence recursively where `Fn = Fn-1 + Fn-2`.
- Converts between number systems (binary, octal, hexadecimal) using Python's built-in functions.
</details>

<details>
<summary><h3>Viva Q&A</h3></summary>

**Q1: What are the base cases in the Fibonacci recursive function?**  
> `n=1` returns `0`, and `n=2` returns `1`. These prevent infinite recursion.

**Q2: Why use recursion instead of iteration?**  
> Recursion provides a cleaner implementation that matches the mathematical definition but is less efficient due to repeated calculations.

**Q3: Explain base 2 and 8 in number conversion.**  
> Base 2 (binary) uses `int(num, 2)`, while base 8 (octal) uses `int(num, 8)`. These represent different number systems.

**Q4: How does Python handle hexadecimal conversion?**  
> Python’s `hex()` function converts an integer to a string with a `0x` prefix. It uses digits `0-9` and letters `a-f` for representation.
</details>

---

## 📊 Program 3: String Analysis 📜

<details>
<summary><h3>Working</h3></summary>

- Analyzes a sentence for word count, digits, uppercase and lowercase letters.
- Compares string similarity by character matching and length ratio.
</details>

<details>
<summary><h3>Viva Q&A</h3></summary>

**Q1: How does the `split()` function help in counting words?**  
> Splits the string at whitespace and returns a list of words. The `len()` of this list gives the word count.

**Q2: Why use `isdigit()` and `isupper()` over ASCII comparisons?**  
> These methods are more Pythonic and handle Unicode, whereas ASCII comparisons are faster but less readable.

**Q3: How is string similarity calculated?**  
> `(Number of matching characters) / (Length of the longer string)` gives the similarity percentage.

**Q4: How are special characters handled?**  
> They are counted separately from letters and digits and affect the total character count but not specific counts.
</details>

---

## 📈 Program 4: Basic Matplotlib Plots 📊

<details>
<summary><h3>Working</h3></summary>

- Creates a bar plot using categories and values with labels and formatting.
- Generates a scatter plot with markers, labels, and a legend.
</details>

<details>
<summary><h3>Viva Q&A</h3></summary>

**Q1: What are the essential Matplotlib components?**  
> Figure, axes, labels (x, y), title, and data points/series.

**Q2: How does the `color` parameter affect plots?**  
> Defines the fill/line color using named colors (e.g., "red") or hex codes. This improves visibility and differentiation.

**Q3: What is the purpose of `plt.show()`?**  
> Renders the plot in a window or notebook. Without it, the plot remains in memory unrendered.

**Q4: Difference between `plot()` and `scatter()`?**  
> `plot()` connects points with lines, while `scatter()` displays individual points. `scatter` is better for visualizing correlations.
</details>

---

## 📊 Program 5: Histogram and Pie Charts 📊

<details>
<summary><h3>Working</h3></summary>

- Creates a histogram from data points with specified bins.
- Generates a pie chart with percentage labels and exploded slices.
</details>

<details>
<summary><h3>Viva Q&A</h3></summary>

**Q1: How do bins affect histogram visualization?**  
> More bins show finer distribution details but may introduce noise. Fewer bins smooth data but may hide patterns.

**Q2: What is the purpose of the `explode` parameter in pie charts?**  
> Separates a slice from the pie chart for emphasis. It takes a tuple of offset values.

**Q3: How does the `autopct` parameter work in pie charts?**  
> Formats percentage labels on pie slices. `%1.1f%%` shows one decimal place with the `%` symbol.

**Q4: Why use `edgecolor` in histograms?**  
> Improves visibility by defining bin boundary colors when bins have the same fill color.
</details>

---

## 📈 Program 6: Linear Plotting 📉

<details>
<summary><h3>Working</h3></summary>

- Creates a basic line plot with markers.
- Demonstrates multiple line plots with different styles.
</details>

<details>
<summary><h3>Viva Q&A</h3></summary>

**Q1: Available line styles in Matplotlib?**  
> Solid (`-`), dashed (`--`), dotted (`:`), dash-dot (`-.`).

**Q2: How does the `marker` parameter work?**  
> Adds points at data locations. Examples: `'o'` (circle), `'s'` (square), `'^'` (triangle).

**Q3: Purpose of `legend()`?**  
> Displays plot labels, which is essential for identifying multiple series.

**Q4: How do you handle multiple plots?**  
> Use `subplots()` or multiple `plot()` calls with different styles/colors.
</details>

---

## 📊 Program 7: Seaborn Customization 🐧

<details>
<summary><h3>Working</h3></summary>

- Uses the `tips` dataset to demonstrate Seaborn's statistical visualization capabilities.
- Implements customization options for better visualization.
</details>

<details>
<summary><h3>Viva Q&A</h3></summary>

**Q1: Difference between Seaborn and Matplotlib?**  
> Seaborn provides statistical visualization with better defaults and built-in themes, while Matplotlib is more general.

**Q2: Why convert data to categorical types?**  
> Improves memory usage, enables categorical operations, and ensures proper ordering in plots.

**Q3: What is the purpose of `countplot()`?**  
> Displays the frequency of categorical variables. Useful for analyzing distributions.

**Q4: How does the `hue` parameter affect plots?**  
> Adds a third variable via color coding, enabling multivariate visualizations.
</details>


## 📊 Program 8: Pandas Basics 🐼

<details>
<summary><h3>Working</h3></summary>

- Demonstrates loading and analyzing datasets with Pandas.
- Performs basic operations like filtering, grouping, and aggregating data.
</details>

<details>
<summary><h3>Viva Q&A</h3></summary>

**Q1: What is the role of the `DataFrame` in Pandas?**  
> A `DataFrame` is a 2D labeled data structure similar to an Excel sheet. It is the core data object in Pandas.

**Q2: How does the `groupby()` function work?**  
> Splits data into groups based on column values, allowing you to apply aggregate functions like `sum`, `mean`, or `count`.

**Q3: Difference between `iloc` and `loc`?**  
> `iloc` selects rows/columns by index position, while `loc` selects them by labels.

**Q4: How does Pandas handle missing data?**  
> Missing values are represented as `NaN`. You can handle them using `fillna()` (replace with a value) or `dropna()` (remove them).
</details>

---

## 📊 Program 9: Advanced Data Visualization 📉

<details>
<summary><h3>Working</h3></summary>

- Combines Seaborn and Matplotlib for complex visualizations.
- Creates a heatmap to show correlations.
- Uses pair plots to explore relationships between multiple variables.
</details>

<details>
<summary><h3>Viva Q&A</h3></summary>

**Q1: What is a heatmap used for?**  
> A heatmap visually represents data values as a matrix with varying colors. It's commonly used to display correlations or distributions.

**Q2: How is a pair plot different from a scatter plot?**  
> A pair plot generates scatter plots for all variable combinations in a dataset, making it ideal for exploratory analysis.

**Q3: Explain the `annot=True` parameter in heatmaps.**  
> Displays numerical values directly on the heatmap cells for clarity.

**Q4: How does the `cmap` parameter affect the heatmap?**  
> Changes the color scheme, e.g., `cmap='coolwarm'` for gradients ranging from cool to warm tones.
</details>

---

## 📊 Program 10: Interactive Dashboards 🕹️

<details>
<summary><h3>Working</h3></summary>

- Builds an interactive dashboard using Plotly and Dash.
- Allows users to dynamically filter and visualize data.
</details>

<details>
<summary><h3>Viva Q&A</h3></summary>

**Q1: What is Plotly?**  
> Plotly is a Python library for interactive visualizations like line plots, scatter plots, and dashboards.

**Q2: How does Dash differ from Matplotlib and Seaborn?**  
> Dash focuses on creating web-based, interactive dashboards, while Matplotlib and Seaborn are static visualization tools.

**Q3: What are callbacks in Dash?**  
> Callbacks enable interactivity by updating charts or UI elements in response to user input.

**Q4: Explain the importance of layout in Dash apps.**  
> The layout defines the structure of the dashboard, including HTML components and graphs.
</details>
