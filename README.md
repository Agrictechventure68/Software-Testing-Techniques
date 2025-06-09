# Software-Testing-Techniques

🧠 What is Static Testing?
Static Testing is a software testing technique performed without executing the code.
It focuses on reviewing code, documentation, and design to find errors early in the development cycle.

🎯 Key Objectives:
Identify bugs before runtime

Improve code quality

Reduce development cost and time

Encourage collaborative improvement

📘 Types of Static Testing Techniques
Technique	Description
1. Reviews	Team members manually examine code, documents, or requirements to identify issues. Can be informal.
2. Walkthroughs	The author guides team members through the product to gather feedback and ensure understanding.
3. Inspections	A formal process involving roles (moderator, reviewer, author) and detailed defect detection procedures.
4. Static Analysis	Use of automated tools to scan code for potential issues like security flaws, logic errors, or standard violations.
5. Linting	A type of static analysis that detects code style issues, formatting errors, and syntax problems.

🔧 Tools Used in Static Testing
Here are some popular tools that help automate static testing:

Tool	Language Support	Purpose
SonarQube	Java, Python, JS, etc.	Detects bugs, vulnerabilities, code smells
Pylint	Python	Finds errors, enforces coding standards
Flake8	Python	Checks syntax, style, complexity
ESLint	JavaScript, TypeScript	Flags problematic patterns in JavaScript code
Checkstyle	Java	Ensures Java code follows style conventions
Cppcheck	C/C++	Detects undefined behavior, memory leaks
CodeClimate	Multi-language	Quality metrics + GitHub integration

🧩 Real-World Example
Scenario:
A developer writes a Python function with some poor naming conventions and a bug.

python
def Adder(x,y):
   return x - y   # ❌ Logical error
Detected By: Pylint

bash
$ pylint calculator.py
calculator.py:1:0: C0103: Function name "Adder" doesn't conform to snake_case (invalid-name)
calculator.py:2:11: W0612: Subtraction used instead of addition (possible bug)
✔️ Issue found without running the code!
Static testing catches bugs before execution — saving time and avoiding failure in production.

💡 Why Static Testing Matters
Benefit	Explanation
✅ Early Detection	Find issues before running code — before it gets expensive to fix.
✅ Improved Collaboration	Teams share feedback on code and design through walkthroughs and reviews.
✅ Documentation Accuracy	Ensures requirements/specifications are consistent and clear.
✅ Security & Quality	Tools catch vulnerabilities and enforce secure coding practices.
✅ Supports Continuous Delivery	Keeps the code clean and testable for CI/CD pipelines.

📦 Assignment Folder Structure (Optional for Submission)
javascript

static-testing-assignment/
├── README.md               ← Contains all explanation (this document)
├── calculator.py           ← Sample buggy function (for demo)
└── pylint_output.txt       ← (Optional) Output from static analysis
🎯 Conclusion
Static Testing empowers teams to:

Catch errors early 🐛

Improve collaboration 🤝

Write cleaner, more secure code 🔐

From manual reviews to automated tools, it plays a crucial role in developing reliable software before a single line is executed. 🚀

