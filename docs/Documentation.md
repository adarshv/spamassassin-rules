# Documentation for SpamAssassin Rules Repository

This document provides detailed information about the SpamAssassin Rules Repository, including usage instructions, rule categories, testing procedures, and contributor guidelines.

## Table of Contents

1. [Usage Instructions](#usage-instructions)
2. [Rule Categories](#rule-categories)
3. [Testing Procedures](#testing-procedures)
4. [Contributor Guidelines](#contributor-guidelines)

## Usage Instructions

1. **Adding Rules:**
   - To add new rules, create a `.cf` file under the appropriate category in the `/rules` directory.
   - Follow the SpamAssassin rule format (`body`, `score`, `describe`).
   - Ensure the `score` values match your desired spam threshold.

2. **Rule Categories:**
   - Rules are categorized into different subdirectories within the `/rules` directory based on their purpose (e.g., header, body, URIBL).
   - Maintain a clear and organized structure when adding or updating rules.

3. **Updating Rules:**
   - If updating existing rules, modify the corresponding `.cf` file in the `/rules` directory.
   - Update the `score` and `describe` directives as necessary.

4. **Testing Rules:**
   - Test your rules using relevant test cases in the `/tests` directory.
   - Use the TAP (Test Anything Protocol) format for test cases.
   - Run SpamAssassin tests to validate rule effectiveness.

5. **Documentation Updates:**
   - Update the `README.md` file with any changes to rules, test cases, or usage instructions.
   - Ensure the documentation is accurate and up-to-date.

## Rule Categories

The SpamAssassin rules are categorized into the following directories within the `/rules` directory:

- `header`: Rules related to email header analysis.
- `body`: Rules targeting content in the email body.
- `uri`: Rules for analyzing URIs and links.
- `uribl`: Rules using URIBL (Uniform Resource Identifier Blacklist) for spam detection.

Feel free to create additional subdirectories or categories as needed to organize rules effectively.

## Testing Procedures

1. **Test Cases:**
   - Create test cases in the `/tests` directory using the TAP format.
   - Ensure test cases cover various scenarios to validate rule behavior comprehensively.

2. **Running Tests:**
   - Use the `spamassassin` command-line tool to run tests against your rules and test cases.
   - Verify that the rules correctly identify spam or non-spam emails based on expectations.

3. **Automation (Optional):**
   - Consider automating the testing process using scripts to streamline testing and ensure consistent results.

## Contributor Guidelines

1. **Getting Started:**
   - Fork the repository and clone it to your local machine.
   - Create a new branch for your contributions.

2. **Adding Rules:**
   - Follow the guidelines outlined in the `CONTRIBUTING.md` file for adding or updating rules.
   - Maintain code style, clear descriptions, and meaningful commit messages.

3. **Submitting Pull Requests (PRs):**
   - Submit PRs from your forked repository to the main repository for review and integration.
   - Be open to feedback and collaborate with maintainers and contributors for improvements.

4. **License Agreement:**
   - By contributing, you agree that your contributions will be licensed under the [MIT License](./LICENSE.md).

For more detailed guidelines and instructions, refer to the `CONTRIBUTING.md` file.

## Contact

For any questions, feedback, or assistance regarding the SpamAssassin Rules Repository, feel free to contact us at [hello@adarshv.com](mailto:hello@adarshv.com).
