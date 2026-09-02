# Day 02 — Prompt Engineering

## 📌 Topic

- Lazy Prompt vs Engineering Prompt
- Prompt Iteration
- Zero-shot Prompting
- One-shot Prompting
- Few-shot Prompting

---

## 1. What is a Prompt?

A prompt is an instruction, question, or input given to an AI model to get a desired output.

Example:

> Explain Machine Learning.

This is a simple prompt, but it does not provide much context or guidance.

---

## 2. Lazy Prompt vs Engineering Prompt

### Lazy Prompt

A lazy prompt is vague and gives very little information about what we actually want.

Example:

> Explain Machine Learning.

The AI has to decide the audience, depth, format, examples, and style by itself.

### Engineering Prompt

An engineering prompt gives the AI clear instructions, context, requirements, and output expectations.

Example:

> Explain Machine Learning to a 10-year-old as a teacher. Use simple language and real-world examples. Explain what it is, how it works, and where it is used. Present the answer step-by-step.

### Key Difference

| Lazy Prompt | Engineering Prompt |
|---|---|
| Vague | Specific |
| Less context | More context |
| Output can be unpredictable | Output is more controlled |
| Simple instruction | Task + context + constraints |

---

## 3. Prompt Iteration

Prompt engineering is not always about creating the perfect prompt in the first attempt.

A useful process is:

**Prompt V1 → Get Output → Identify Problems → Improve Prompt → Prompt V2 → Better Output**

### Example

Instead of:

> Create my resume.

I created a more detailed prompt:

> Create a professional one-page resume for an AI Engineering fresher. Use only the information I provide. Do not add unnecessary or imaginary information. Include Professional Summary, Education, Skills, Projects, Experience, and Interests/Hobbies. Make it ATS-friendly. Use a professional format and highlight my actual projects and skills.

The second prompt gives the AI much clearer requirements.

---

## 4. Zero-shot Prompting

Zero-shot prompting means asking the AI to perform a task without providing examples.

### Example

> Categorize this student as Excellent, Good, or Needs Improvement based on their marks and attendance.

No examples are provided.

**Zero examples → Zero-shot**

---

## 5. One-shot Prompting

One-shot prompting means providing one example before giving the new task.

### Example

```text
Example:
Marks: 95
Attendance: 90%
Category: Excellent

Now classify:
Marks: 87
Attendance: 74%
Category: ?


## 6. Few-shot Prompting

Few-shot prompting means providing a small number of examples before asking the AI to handle a new input.

Example
Student 1:
Marks: 95
Attendance: 90%
Category: Excellent

Student 2:
Marks: 75
Attendance: 89%
Category: Good

Student 3:
Marks: 40
Attendance: 52%
Category: Needs Improvement

Now classify:
Marks: 87
Attendance: 74%
Category: ?

The AI studies the examples and identifies the pattern before generating the category for the new student.

Important Point

Few-shot does not have to mean exactly 2 or 3 examples. It means giving the model a small number of examples to guide its response.

### 7. Zero-shot vs Few-shot
Zero-shot	Few-shot
No examples	A few examples
AI follows the instruction directly	AI follows the demonstrated pattern
Less guidance	More guidance
Useful for straightforward tasks	Useful when examples clarify the expected output
🧠 What I Learned
A prompt is an instruction given to an AI model.
Clear prompts generally provide better control over the output.
Prompt engineering involves improving prompts through iteration.
Zero-shot prompting uses no examples.
One-shot prompting uses one example.
Few-shot prompting uses a small number of examples.
Examples can help an AI understand the expected pattern and output format.
🛠️ Practice

I practiced prompt engineering using a student classification problem based on:

Marks
Attendance
Expected category

I created examples for:

Excellent
Good
Needs Improvement

Then I provided a new student's data and asked the AI to predict the category.

🎯 Key Takeaway

Better instructions + useful context + clear examples = better-controlled AI outputs.