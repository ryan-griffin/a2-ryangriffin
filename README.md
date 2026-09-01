# Due Soon

Due Soon is a single-page assignment tracker for WPI students. The responsive layout uses CSS Grid for the main page structure and Flexbox for form controls and smaller layout elements.

**Live site:** https://a2-ryangriffin.onrender.com/

## Features

- Displays the complete assignment dataset stored on the server
- Adds and deletes assignments without reloading the page
- Calculates `daysRemaining` and `urgency` on the server using each assignment's due date and priority
- Uses an external stylesheet with element, ID, and class selectors

## Technical Achievements

- **Single-page application:** The form and complete dataset appear on the same page. After every add, edit, or delete request, the server returns the updated dataset and the browser redraws the table without reloading.
- **Modify existing data:** Each row has an Edit button that loads its values into the form. Submitting the edited assignment sends a `PUT` request, and the server validates the changes and recalculates its derived fields before updating the dataset.
