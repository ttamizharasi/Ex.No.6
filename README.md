#  Ex.No.6 – Development of Python Code Compatible with Multiple AI Tools

### Name: Tamizharasi S
### Register no: 212222040170
 
## Aim:
Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights using Multiple AI Tools.


##  AI Tools Required
- ChatGPT  
- Claude  
- Gemini (Google Bard)  
- Optional: Cohere, Meta LLaMA APIs (for extension)


##  Explanation
This experiment explores how to develop Python code that interacts with multiple AI APIs and evaluates the persona prompting technique. The persona chosen is that of a *Programmer*, and various Python tasks were given as prompts across different AI tools. Outputs were analyzed in terms of correctness, clarity, efficiency, and learning support. This comparison allows users to determine the best AI tool for specific programming-related problems and scenarios.



##  Subtopics with Detailed Prompt Analysis

| No. | Subtopic | AI Prompt | Output Comparison | Inference |
|-----|----------|-----------|-------------------|-----------|

### 1. Generate Python MCQs
- **Prompt:** Create 5 MCQs in Python with answers.
- **ChatGPT Output:** Neatly formatted with options and correct answers.
- **Claude Output:** Similar output, but some answers lacked clarity.
- **Gemini Output:** Included questions but lacked consistent format.

**Answer:**  
MCQ generation is helpful for quizzes. ChatGPT provides a user-friendly layout, making it ideal for direct use in exams or e-learning tools. Claude and Gemini can generate questions, but formatting and clarity may need manual tweaking.


### 2. Generate Python Interview Questions
- **Prompt:** Give top 5 Python interview questions with answers.
- **ChatGPT Output:** Gave concise, clear Q&A.
- **Claude Output:** Provided more technical depth.
- **Gemini Output:** Some questions were vague.

**Answer:**  
Interview questions require clarity and relevance. ChatGPT balances both, while Claude offers advanced detail useful for experienced candidates. Gemini underperforms in focus and depth.

### 3. Explain Python Code
- **Prompt:** Explain the following Python code...
- **ChatGPT Output:** Well-structured explanation.
- **Claude Output:** Explains in a more theoretical way.
- **Gemini Output:** Short but correct explanation.

**Answer:**  
Code explanation depends on clarity and user level. ChatGPT gives digestible chunks. Claude helps for deeper understanding, while Gemini stays brief and best for quick checks.


### 4. Fix a Bug in Code


- **Prompt:** Fix the bug in the provided code snippet.
- **All Outputs:** All tools fixed the error correctly.

**Answer:**  
All three tools perform equally well in bug fixing. However, ChatGPT typically includes cleaner and more professional coding practices.


### 5. Convert Python Code to Java
- **Prompt:** Convert Python code to Java.
- **ChatGPT Output:** Accurate and easy-to-follow Java code.
- **Claude Output:** Sometimes skipped small Python-specific syntax.
- **Gemini Output:** Missed class structure at times.

**Answer:**  
ChatGPT excels in cross-language conversion. Claude offers good translation but may confuse new users. Gemini needs refinement in structure.


### 6. Compare Two Algorithms in Python
- **Prompt:** Compare Bubble Sort and Merge Sort in code and time.
- **ChatGPT Output:** Code + time complexity explained.
- **Claude Output:** Focused more on theory.
- **Gemini Output:** Lacked implementation details.

**Answer:**  
ChatGPT gives balanced insights. Claude provides theoretical background, good for oral exams. Gemini lacks completeness.


### 7. Add Comments to Code
- **Prompt:** Add comments to a given code.
- **ChatGPT Output:** Accurate and helpful.
- **Claude Output:** More educational comments.
- **Gemini Output:** Incomplete in parts.

**Answer:**  
Claude is best for learning through comments. ChatGPT focuses on concise and necessary explanations. Gemini can miss out on deeper context.


## Real Time Implementation:

### 8. Create a Flask Web App
- **Prompt:** Build a Flask app that calculates the BMI (Body Mass Index) using Python3.

**Answer:**  
![image](https://github.com/user-attachments/assets/9560951d-b57f-45a1-bedf-08993d15db56)

app.py:
```py
from flask import Flask, render_template, request, redirect, url_for

app = Flask(__name__)

# In-memory task list
tasks = []

@app.route('/')
def index():
    return render_template('index.html', tasks=tasks)

@app.route('/add', methods=['POST'])
def add():
    task = request.form.get('task')
    if task:
        tasks.append(task)
    return redirect(url_for('index'))

@app.route('/delete/<int:task_id>')
def delete(task_id):
    if 0 <= task_id < len(tasks):
        tasks.pop(task_id)
    return redirect(url_for('index'))

if __name__ == '__main__':
    app.run(debug=True)


### 9. Explain Python Decorators

| Tool     | Example Included | Concept Clarity | Real-World Use |
|----------|------------------|-----------------|----------------|
| ChatGPT  | ✅               | Medium          | Basic          |
| Claude   | ✅✅             | High            | Good           |
| Gemini   | ✅               | Medium          | High           |

- **Prompt:** Explain Python decorators with an example.

**Answer:**  
Claude excels with deep conceptual understanding. ChatGPT is minimal. Gemini offers multiple use cases. Claude is ideal for interviews.



##  Summary Table – Best AI Tool by Subtopic

| Subtopic | Best Tool | Reason |
|----------|-----------|--------|
| MCQs | ChatGPT | Structured formatting |
| Interview Qs | Claude | Deeper explanations |
| Code Explanation | ChatGPT | Clear breakdown |
| Bug Fix | All | Equal performance |
| Python to Java | ChatGPT | Clean structure |
| Quiz App | Claude | Logical clarity |
| Algorithm Compare | ChatGPT | Balanced insights |
| Add Comments | Claude | Best for learners |
| Regex | ChatGPT | Clean regex |
| Try-Except | Claude | Conceptual clarity |
| File Handling | ChatGPT | Efficient |
| GUI Tkinter | Gemini | Validation included |
| Flask App | ChatGPT | Uses templates |
| Decorators | Claude | Deep conceptual |
| CSV to JSON | Gemini | Robust |
| Email | Gemini | Secure config |
| Matplotlib | Gemini | Neat visuals |
| List Comprehension | Claude | Educational |
| Class & Object | Claude | Better for learning |
| Recursion | Claude | Concept clarity |


## Conclusion
This experiment successfully demonstrated how Python code can be developed using prompts across multiple AI platforms. Each tool—ChatGPT, Claude, and Gemini—offered unique strengths: ChatGPT for concise implementation, Claude for teaching and depth, and Gemini for user-friendly features and real-world advice. By analyzing the generated outputs, developers can select the best AI tool based on task complexity, use case, and learning goals.


## Result
The corresponding prompt executions across multiple AI tools were successful. All outputs were analyzed and compared, and actionable insights were derived. The experiment fulfilled its objective.
