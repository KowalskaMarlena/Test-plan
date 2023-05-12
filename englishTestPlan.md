# Test plan: Cinema Seat Reservation

## Test objective:

- To verify the correctness and functionality of the cinema seat reservation feature in the application.

## Test Enviroment:

- Operating System: Windows 10
- Web browsers: Google Chrome
- Test data: a set of sample reservation data (valid and invalid).

## Test Scenarios:

### A. Successful Reservation of a Single Seat in the Cinema as a Logged-In User

Precodintiones: The user is logged in and is on the seat selection page.

- Step 1: Select the seat marked in green colour.
- Step 2: Click the "Confirm Reservation" button.

Expected Result: The user receives a confirmation email for the reserved seat with payment details to be made at the cinema before the show.

### B. Successful Reservation of Multiple Seats in the Cinema as a Logged-In User

Precondition: The user is logged in and is on the seat selection page.

- Step 1: Select multiple seats marked in green color.
- Step 2: Click the "Confirm Reservation" button.

Expected Result: The user receives a confirmation email for the reserved seats with payment details to be made at the cinema before the show.

### C. Unsuccessful Seat Reservation as a Guest User

Precondition: The user is not logged in and is on the seat selection page.

- Step 1: Select the seat marked in green color.
- Step 2: Click the "Confirm Reservation" button.

Expected Result: The user is prompted to log in or register if they don't have an account.

### D. Unsuccessful Reservation for a Logged-In User – Selecting an Already Reserved Seat

Precondition: The user is logged in and is on the seat selection page.

- Step 1: Select the seat marked in red color.

Expected Result: An error message is displayed indicating that the selected seat cannot be reserved.

### E. Unsuccessful Reservation due to Inaction

Precondition: The user is on the seat selection page.

- Step 1: Select the seat marked in green color.
- Step 2: Do not click the "Confirm Reservation" button for 5 minutes.

Expected Result: If the user does not click the "Confirm Reservation" button within 5 minutes, they are redirected to the application's homepage. An error message is displayed indicating the failure to complete the reservation for the selected seat.

## Test Procedures:

- Go through each of the test scenarios described above.
- Record the results of each test step, including expected and actual outcomes.
- In case of encountering any errors, document detailed information about the error, such as the error message, steps to reproduce the error, error identifier, etc.

## Test Resources:

- Computer with the required operating system and browser installed.
- Sample seats for reservation (valid and invalid).

## Risks and Considerations:

- Monitor application response time to ensure reservations are being processed in a timely manner.

## Test Schedule:

- Stage 1: Test environment preparation, test data configuration - 2 days.
- Stage 2: Conducting tests - 3 days.
- Stage 3: Analyzing results, reporting defects - 1 day.

## Results Reporting:

- All defects will be reported and logged in the defect management system, including detailed defect information, steps to reproduce, and expected behavior.
