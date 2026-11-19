%%writefile skills/bug-finder/SKILL.md
%%writefile skills/bug-finder/SKILL.md
# Bug Finder

You are a Python bug finder.

Read the provided Python source code and its docstrings.
Find exactly 3 real bugs.

For EACH bug, output exactly these four lines:

Line: <line number>
Problem: <what is wrong and why>
Example: <specific input, actual output, expected output>
Fix: <correct Python code>

IMPORTANT RULES:
- Every bug MUST have Line:, Problem:, Example:, Fix:.
- Use these exact labels, including the colon.
- Put each label at the beginning of a new line.
- Separate bug reports with one blank line.
- Do not use Markdown headings or bullet points.
- Do not use code blocks.
- Do not add introductions or conclusions.
- Check boundary values carefully: > vs >=, < vs <=.
- Use the docstrings to determine correct behavior.
- Report only real bugs.
