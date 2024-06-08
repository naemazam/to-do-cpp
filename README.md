# To-Do List App in C++

## Overview
This is a simple To-Do List application written in C++. The application allows users to create, manipulate, and save a list of tasks. The tasks are stored in a `list.txt` file, enabling persistence across sessions.

## Classes

### TodoList
This class represents the entire to-do list and contains methods to manipulate the list of items.

#### Methods
- **addItem(const Item &item)**: Adds a new item to the list.
- **removeItem(int index)**: Removes an item from the list based on its index.
- **displayItems() const**: Displays all the items in the list.
- **saveToFile() const**: Saves the list of items to `list.txt`.
- **loadFromFile()**: Loads the list of items from `list.txt`.

### Item
This class represents a specific task in the to-do list.

#### Attributes
- **std::string description**: A description of the task.
- **bool completed**: A flag indicating whether the task is completed.

## Libraries Used

### iostream
Used for input and output from the user.

### iomanip
Used for formatting the display of the list items.

### string
Used for managing and formatting user input.

### fstream
Used for reading from and writing to the `list.txt` file.

### stdio
Used for file manipulation, specifically for removing the `list.txt` file.

## Getting Started

### Prerequisites
- A C++ compiler (e.g., g++, clang++)
- A text editor or IDE (e.g., VSCode, CLion)

### Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/naemazam/to-do-cpp.git
    cd to-do-cpp
    ```
2. Compile the application:
    ```sh
    g++ main.cpp -o to-do-cpp
    ```

### Usage
Run the application:
```sh
./to-do-cpp
```

### Example
Upon running the application, you will be presented with a menu to add, remove, display tasks, save the list to a file, or load the list from a file.

## File Structure
- **main.cpp**: The main file containing the entry point of the application.
- **TodoList.h**: Header file for the `TodoList` class.
- **Item.h**: Header file for the `Item` class.
- **list.txt**: File used to store the tasks persistently.
- **README.md**: This README file.

## Future Enhancements
- Add a feature to edit existing tasks.
- Implement a search function to find tasks by keywords.
- Add a graphical user interface (GUI).
