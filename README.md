

# 🎨 Python Data Visualization Programs
<p align="center">
  <img src="/api/placeholder/800/200" alt="Data Visualization Banner">
</p>

## 📊 Program Documentation & Viva Questions

### 🔢 Program 1: Best Test Average and Palindrome Number

<details>
<summary><b>Working</b></summary>

- Accepts three test marks, removes the lowest score, and calculates the average of the best two.  
- Checks if a number is a palindrome using string reversal.  
- Counts the occurrences of each digit in the number.  

</details>

<details>
<summary><b>Viva Questions</b></summary>

**Q1: How does `min()` help in finding the best two scores?**  
> It returns the lowest score, which is subtracted from the total to calculate the best two scores.

**Q2: What happens with non-numeric input?**  
> A `ValueError` is raised, which can be handled using a `try-except` block.

**Q3: Explain `number[::-1]` in palindrome checking.**  
> It uses string slicing with a step of `-1` to reverse the string.

**Q4: How does the digit counting dictionary work?**  
> Iterates through each character, checks if it's a digit, and maintains a count using a dictionary.

</details>

---

### 🔄 Program 2: Fibonacci and Number Conversions

<details>
<summary><b>Working</b></summary>

- Implements the Fibonacci sequence using recursion: `Fn = Fn-1 + Fn-2`.  
- Converts numbers between different bases (binary, octal, hexadecimal).

</details>

<details>
<summary><b>Viva Questions</b></summary>

**Q1: What are the base cases in Fibonacci recursion?**  
> `n=1` returns `0` and `n=2` returns `1` to avoid infinite recursion.

**Q2: Why use recursion instead of iteration?**  
> Recursion offers a cleaner implementation but is less efficient.

**Q3: Explain base 2 and base 8 conversions.**  
> Use `int(num, 2)` for binary and `int(num, 8)` for octal conversions.

**Q4: How does Python handle hexadecimal conversion?**  
> The `hex()` function converts an integer to a string with a `0x` prefix, using digits `0-9` and `a-f`.

</details>

---

## **📊 Program 3: String Analysis and Similarity**
### **Working**
1. **Part A**: 
   - Accepts a sentence as input.
   - Counts the number of words using `split()`.
   - Counts digits, uppercase, and lowercase letters using loops and conditional checks.

2. **Part B**:
   - Compares two strings to calculate similarity.
   - Calculates the ratio of matching characters to the length of the longer string.

### **Viva Q&A**
**Q1: How do you count the number of words in a sentence?**  
> Use the `split()` method to separate words and `len()` to count them.

**Q2: How is string similarity calculated?**  
> `(Number of matching characters) / (Length of the longer string)` gives the similarity percentage.

**Q3: How do you identify uppercase and lowercase letters?**  
> Use conditions `'A' <= ch <= 'Z'` for uppercase and `'a' <= ch <= 'z'` for lowercase.

---

## **📊 Program 4: Matplotlib Visualizations**
### **Working**
1. **Part A**: Demonstrates bar plots using `plt.bar()`.
2. **Part B**: Demonstrates scatter plots using `plt.scatter()`.

### **Viva Q&A**
**Q1: What is the purpose of `plt.bar()`?**  
> It creates bar plots to compare categorical data.

**Q2: How do scatter plots differ from line plots?**  
> Scatter plots show individual data points, while line plots connect them.

**Q3: How do you customize the plots?**  
> Use attributes like `color`, `title`, and `xlabel()`.

---

## **📊 Program 5: Histograms and Pie Charts**
### **Working**
1. **Part A**: Generates histograms using `plt.hist()`.
2. **Part B**: Creates pie charts with labels and percentages using `plt.pie()`.

### **Viva Q&A**
**Q1: What is the purpose of a histogram?**  
> It visualizes data distribution across bins.

**Q2: How do you highlight a slice in a pie chart?**  
> Use the `explode` parameter to separate a slice.

---

## **📈 Program 6: Linear Plotting**
### **Working**
1. **Part A**: Demonstrates linear plotting using `plt.plot()`.
2. **Part B**: Shows line formatting using markers, colors, and styles.

### **Viva Q&A**
**Q1: What is the default line style in `plt.plot()`?**  
> A solid line.

**Q2: How do you add markers to a line plot?**  
> Use the `marker` parameter, e.g., `'o'` for circles.

---

## **📊 Program 7: Customizing Seaborn Plots**
### **Working**
- Utilizes Seaborn's aesthetics and `sns.countplot()` for count-based visualizations.
- Allows customization using attributes like `palette`, `style`, and `order`.

### **Viva Q&A**
**Q1: How does Seaborn differ from Matplotlib?**  
> Seaborn simplifies statistical visualization and offers built-in themes.

**Q2: What is the purpose of `sns.set_theme()`?**  
> It sets the overall style for plots.

---

## **📊 Program 8: Bokeh Visualizations**
### **Working**
1. **Part A**: Demonstrates line graphs with annotations and legends using `bokeh.plotting`.
2. **Part B**: Creates various plots (line, scatter, bar) and arranges them using layouts.

### **Viva Q&A**
**Q1: How is Bokeh different from Matplotlib?**  
> Bokeh creates interactive, browser-based visualizations, while Matplotlib focuses on static plots.

**Q2: How do you add annotations in Bokeh?**  
> Use the `Label` class and `add_layout()` method.

---

## **📊 Program 9: 3D Plotting with Plotly**
### **Working**
- Visualizes multidimensional data in 3D using `plotly.express.scatter_3d()`.

### **Viva Q&A**
**Q1: What is the purpose of 3D plots?**  
> They visualize relationships between three variables simultaneously.

**Q2: How do you add color to distinguish categories in Plotly?**  
> Use the `color` parameter in `scatter_3d()`.

---

## **📊 Program 10: Time Series and Maps with Plotly**
### **Working**
1. **Part A**: Time series visualization using `plotly.express.line()`.
2. **Part B**: Creates interactive choropleth maps using `plotly.express.choropleth()`.

### **Viva Q&A**
**Q1: How do you prepare data for time series visualization?**  
> Ensure the date column is in a datetime format.

**Q2: What is a choropleth map?**  
> It visualizes geographical data using color intensities.



## 🛠️ Technologies Used
- Python 3.x  
- Libraries: Matplotlib, Seaborn, Bokeh, Plotly, Pandas, NumPy  

---

## 📚 Prerequisites

Install required libraries using:  
```bash
pip install matplotlib seaborn bokeh plotly pandas numpy
```

---

## 🚀 Getting Started
1. Clone the repository:  
   ```bash
   git clone <repository_url>
   ```
2. Install the dependencies.  
3. Run individual programs as needed.  
4. Refer to the documentation for program-specific details.

---

## 📖 Documentation Structure
Each program includes:  
- **Working Explanation**  
- **Viva Questions and Answers**  
- **Code Examples**  

---

## 🤝 Contributing
Pull requests are welcome! For major changes, open an issue to discuss them first.

---

## 📝 License
This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).

