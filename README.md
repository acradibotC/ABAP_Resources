# ABAP Resources for Writing Testable Code

This repository contains ABAP code examples, exercises, and reference implementations based on the official SAP Learning course: **[Writing Testable Code for ABAP](https://learning.sap.com/courses/writing-testable-code-for-abap)**.

It serves as a practical, hands-on companion to the course, allowing you to see the concepts in a real system and experiment with them directly.

---

## About This Repository

The primary goal of this repository is to provide a working code base that demonstrates the principles of software craftsmanship and modern ABAP development. While the SAP Learning course provides excellent theoretical knowledge and short examples, this repository aims to be the place where you can pull the complete, working code into your own development environment.

Whether you are following along with the course or just want to explore best practices for testable ABAP code, you'll find valuable resources here.

## Key Concepts Covered

The code in this repository demonstrates several critical concepts for writing clean, maintainable, and testable ABAP code:

-   **Test-Driven Development (TDD):** The practice of writing tests *before* writing the production code.
-   **ABAP Unit:** A deep dive into the ABAP unit testing framework.
-   **Test Doubles:** Creating and using Mocks, Stubs, and Fakes to isolate the code you are testing.
-   **Dependency Injection:** How to decouple your objects to make them easier to test and reuse.
-   **Refactoring:** Techniques for safely improving the design of existing legacy code.
-   **Clean ABAP:** Applying principles from the [Clean ABAP style guide](https://github.com/SAP/styleguides/blob/main/clean-abap/CleanABAP.md) to create more readable and maintainable programs.

## Prerequisites

To use the code in this repository, you will need:

1.  **An SAP System:** An on-premise S/4HANA system, a Steampunk (BTP ABAP Environment) system, or a developer edition (like the [ABAP Platform 1909, Developer Edition](https://developers.sap.com/tutorials/abap-platform-1909-setup.html)). Most examples are compatible with ABAP release `7.52` or higher.
2.  **abapGit:** The `abapGit` client must be installed in your SAP system. This is the standard tool for sharing ABAP code via Git. If you don't have it, you can find installation instructions here: [abapGit Installation Guide](https://docs.abapgit.org/guide-installation.html).
3.  **Developer Authorizations:** Your SAP user needs the necessary rights to create and modify ABAP development objects (packages, classes, etc.).

## Getting Started / Installation

You can import the code into your system using `abapGit`.

1.  Log in to your SAP system.
2.  Run the **`abapGit`** report using transaction `ZABAPGIT` or by executing the program directly.
3.  Click on the **"+ New Online"** button.
4.  Enter the following URL in the "Git repository URL" field:
    ```
    https://github.com/acradibotC/ABAP_Resources
    ```
5.  `abapGit` will propose a package name (e.g., `ZABAP_RESOURCES`). You can use this or choose your own local package (e.g., starting with `$`).
6.  Click **"Create Package"**.
7.  Click the **"Pull"** button to download the repository objects into your SAP system.

The code will be downloaded and activated automatically. You can now explore the classes, run the unit tests, and start experimenting!

## Repository Structure

The code is organized into ABAP packages within the `src` folder, following the `abapGit` standard.

-   `/src`: Contains all the ABAP source code.
    -   `zcl_demo_testable_code.clas.abap`: An example of a main class.
    -   `zcl_demo_testable_code.clas.testclasses.abap`: The corresponding local test classes for the main class, demonstrating ABAP Unit tests.

You can view the main classes in the ABAP Development Tools (ADT) for Eclipse or via transaction `SE24`/`SE80`. The corresponding unit tests can be executed directly from ADT (Right-click -> Run As -> ABAP Unit Test) or via the Code Inspector.

## How to Contribute

Contributions are welcome! If you find a bug, have a suggestion for an improvement, or want to add another example, feel free to:

1.  **Open an Issue:** Describe the bug or your suggestion.
2.  **Submit a Pull Request:**
    -   Fork the repository.
    -   Create a new branch for your feature or bugfix.
    -   Make your changes.
    -   Submit a pull request with a clear description of your changes.

Please try to follow the existing coding style and ensure all tests pass before submitting a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

-   A huge thank you to **SAP Learning** for creating the excellent and free course "Writing Testable Code for ABAP."
-   The ABAP community for developing and maintaining incredible open-source tools like `abapGit`.
