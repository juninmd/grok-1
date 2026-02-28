```markdown
# AGENTS.md - AI Coding Agent Guidelines

These guidelines outline the specific principles and rules for development of AI coding agents within this repository.  Adherence to these principles is crucial for maintainability, reliability, and productivity.

## 1. DRY (Don't Repeat Yourself)

- All code should be encapsulated within individual files, each representing a specific component or functionality.
- Avoid duplicating logic or data structures across multiple files.
- Leverage existing components and modules whenever possible to minimize redundancy.

## 2. KISS (Keep It Simple, Stupid)

- Code should be as concise and readable as possible.
- Avoid unnecessary complexity.
- Prioritize clarity over brevity unless there’s a compelling performance reason to deviate.
- Use clear and descriptive variable and function names.

## 3. SOLID Principles

- **Single Responsibility Principle:** Each class/module should have one, and only one, reason to change.  Minimize cohesion.
- **Open/Closed Principle:** The system should be open for extension but closed for modification.  New functionality shouldn't require modifying existing code.
- **Liskov Substitution Principle:**  Subclasses should be substitutable for their base classes without altering the correctness of the program.
- **Interface Segregation Principle:** Clients shouldn't be forced to depend on methods they don’t use.
- **Dependency Inversion Principle:** High-level modules should be dependent on low-level modules, and modules should be dependent on abstractions.

## 4. YAGNI (You Aren’t Gonna Need It)

-  Implement only the features that are currently required.  Avoid premature optimization.
-  Focus on the core functionality of the agent.  Don’t build unnecessary features.
-  Refactor and improve the code as requirements evolve, rather than attempting to build complete features.

## 5. Development Process & Code Structure

- **File Structure:** All files must be organized with a clear hierarchical structure. Use a naming convention that is consistent across the project.
- **Code Style:**  Follow a consistent code style (e.g., PEP 8 for Python).  Use a linter to enforce style compliance.
- **Documentation:**  Provide clear and concise documentation within each file, explaining its purpose and usage.  Consider using docstrings for functions and classes.
- **Test Driven Development:** All new code must be accompanied by comprehensive unit tests.
- **Unit Testing:** Each module should have its own test suite. Tests should cover all critical functionality.
- **Code Reviews:**  All changes must be reviewed by at least one other team member before integration.
- **Commit Frequency:**  Make small, frequent commits.
- **Branching Strategy:** Use a well-defined branching strategy (e.g., Gitflow) to manage development and feature isolation.

## 6. Code Length Constraints

- All code must be maintained to a maximum of 180 lines of code.
-  Avoid excessively large functions or classes.

## 7.  Testing Requirements

- **Unit Tests:** All code must have at least 80% coverage achieved through unit tests.
- Test cases must be clearly defined and easily runnable.
-  Tests should verify edge cases and error handling.
-  Regression tests must be performed after every code change.
-   Test coverage reports must be generated automatically.

## 8.  AGENTS.md Format & Content

- The file should contain clear, concise, and well-commented code.
- Function/method names should be meaningful and follow standard naming conventions.
- Variables should have appropriate data types and potential for type hints.
-  All code should be easily readable and understandable.

-  Example:
    ```python
    # AGENTS.md
    # This file contains the code for the Agent's core logic.

    def process_data(data):
        """
        Processes the provided data.

        Args:
            data: A dictionary containing the data to be processed.

        Returns:
            A processed dictionary.
        """
        # Implementation logic here
        return data  # Placeholder

    def main():
        """
        The main function that orchestrates the Agent's operations.
        """
        data = {"input": "Some data"}
        result = process_data(data)
        print(result)
    ```
```

Goal: To establish a high-quality, maintainable, and reliably functional AI coding agent framework through strict adherence to the guidelines outlined above.
```