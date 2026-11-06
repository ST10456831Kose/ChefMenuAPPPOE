# Chef's Menu Manager - Final POE (Part 3)

## Project Description
The Chef's Menu Manager is a mobile application built using React Native (Expo). This final iteration enhances the application created in Part 2 by introducing full CRUD functionality, advanced search and filtering, dynamic statistics, and a heavily refactored, user-friendly interface.

## 🎥 Video Demonstration
*(As per the submission guidelines, here is the link to the unlisted YouTube video demonstrating the app's functionality)*:


---

## 🚀 Features Implemented

### 1. Manage Menu Items
*   **Create:** Chefs can add new menu items with a name, description, price, and course category.
*   **Update:** Existing menu items can be edited and saved, with the UI updating instantly.
*   **Delete:** Items can be removed from the menu via a confirmation alert to prevent accidental deletions.

### 2. Search and Filter
*   **Search:** A dynamic search bar allows the chef to find items instantly by typing the item's name.
*   **Filter:** A dropdown menu allows filtering items by course (Starter, Main Course, Dessert).
*   **Clear:** A dedicated "Clear" button resets both the search query and the filter to show all items again.

### 3. Menu Statistics
A dedicated statistics card displays real-time data based on the current menu:
*   Total number of menu items.
*   The average price of all items.
*   The total count of items available in each course (Starters, Mains, Desserts).

---

## 📝 Changelog (Changes Since Part 2 & Refactoring)

The application was significantly refactored to meet best practices for mobile development and to satisfy the requirements of Part 3.

### Added Features
*   Implemented a global state management system using React Context API (`MenuContext.js`).
*   Added real-time search functionality.
*   Added filtering by course categories.
*   Added a dynamic statistics calculation card.
*   Implemented form validation (ensuring prices are valid numbers and fields are not empty).

### Refactoring & Enhancements (Requirement 4)
*   **Code Organization:** Reorganized the project into a professional `src` folder structure (`components`, `screens`, `context`).
*   **Reusable Components:** Extracted UI elements into separate, reusable files to reduce code duplication:
    *   `MenuItemCard.js` (Handles the UI for individual menu list items).
    *   `MenuItemForm.js` (Reusable modal used for both adding and editing items).
    *   `StatsCard.js` (Dedicated component for displaying menu statistics).
*   **UI/UX Improvements:** 
    *   Improved the overall layout and spacing for a cleaner look.
    *   Added standard `Alert.alert` popups to provide users with meaningful success and error feedback (e.g., "Item added successfully", "Are you sure you want to delete?").
    *   Added standard button colors and consistent styling across all screens.
*   **Meaningful Naming:** Ensured all variables, functions, and file names follow clear, semantic naming conventions.

---

## 🛠️ How to Run the App

To run this project locally, ensure you have Node.js and Expo CLI installed.

1. Clone this repository or download the code.
2. Open your terminal in the project folder and install dependencies:
   ```bash
   npm install
