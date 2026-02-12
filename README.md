# Stack-Based Line Management Utility (STL Implementation)

This C++ application is a robust utility for managing text lines using the **LIFO (Last In, First Out)** principle. It leverages the C++ Standard Template Library (STL) to provide efficient stack operations and advanced file processing capabilities.

###  Logic & Data Structures
The program is built around the `std::stack<std::string>` container, which manages text lines extracted from files.

**Key Algorithmic Concepts:**
* **LIFO Processing:** Lines are pushed onto the stack as they are read, meaning the last line of the file becomes the first line available for processing. 
* **Stack Reversal:** The utility can reverse the order of elements, effectively restoring the original file sequence or creating new arrangements.
* **Dynamic Renumbering:** Includes logic to prepend line indices to text content, both within the stack and during file-to-file duplication.

###  Key Features
* **STL Integration:** Uses `std::stack` and `std::vector` for modern, safe, and efficient data management.
* **Advanced File I/O:** Features a custom `LineReader` class to wrap `std::getline`, ensuring clean and reliable text ingestion. 
* **Automated File Replication:** Includes a `makeRenumberedCopy` function that reads a source file and generates a new, indexed version in one step.
* **Interactive Console UI:** A menu-driven interface allows users to load, view, reverse, and clear data dynamically.

###  Technical Stack
* **Language:** C++
* **Standard Library:** `<stack>`, `<vector>`, `<fstream>`, `<sstream>`.
* **Architecture:** Object-Oriented Design with specialized classes for data reading and storage.

###  How to Use
1. Prepare a text file (e.g., `3.txt` or `5.txt`) in the project directory.
2. Run the application and choose "Load file into stack" to see the LIFO effect.
3. Use the "Renumber" or "Reverse" options to manipulate the stored lines.
4. Choose "Create renumbered copy" to generate a new file with persistent line indices.
