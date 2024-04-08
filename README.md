# testing-strategy
This is part of an application process. The goal is to show my knowledge on creating robust testing strategies for an specific product to cover most scenarios of a single functionality

# Overall Tasks and Subtasks to every E2E strategy (Test cases only apply to Search Box functionality)

- [ ] **Prepare Test Environment**
  - [ ] Set up testing server 
  - [ ] Install necessary software and tools
  - [ ] Configure network settings
  - [ ] Prepare test data
- [ ] **Develop Test Plan** #Planning
  - [ ] Identify test objectives
  - [ ] Define test scope
  - [ ] Determine testing strategy
  - [ ] Allocate resources and set timeline
  - [ ] Prepare test schedule
- [ ] **Write Test Cases** 
  - [ ] Test Case 1: Check default state of search box
  - [ ] Test Case 2: Verify input functionality of search box
    - [ ] Sub-Case 1: Test with valid input
    - [ ] Sub-Case 2: Test with invalid input
  - [ ] Test Case 3: Check search functionality with various filters
  - [ ] Test Case 4: Validate results page after search execution
- [ ] **Execute Test Cases** 
  1. Run Test Case 1
  2. Run Test Case 2
  - Run Sub-Case 1
  - Run Sub-Case 2
  1. Run Test Case 3
  2. Run Test Case 4
- [ ] **Review Test Results** 
  - [ ] Identify passed and failed cases
  - [ ] Analyze failed cases and identify issues
  - [ ] Document results and issues
- [ ] **Report and Track Issues** 
  - [ ] Create issue report for each identified issue
  - [ ] Submit reports to relevant team
  - [ ] Track progress of issue resolution
- [ ] **Retest and Close Issues** 
  - [ ] Retest fixed issues
  - [ ] Validate fixes and close issues
- [ ] **Update Test Documentation**
  - [ ] Update test plan and cases based on results and changes
  - [ ] Prepare final test report
  - [ ] Archive test documents for future reference

# Test cases definition

| Test Case               | Description                                      | Expected Outcome                                                                                    |
|-------------------------|--------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| Valid One-Way Flight Search | Input valid departure and destination cities, select a valid departure date, click "Search" | Display available flight from Chicago to San Francisco on the specified date. |
| Invalid Departure City  | Input an invalid departure city                  | Display an error message indicating that the departure city is not recognized.                    |
| Invalid Destination City| Input an invalid destination city                | Display an error message indicating that the destination city is not recognized.                  |
| No Available Flights    | Select a date with no available flights          | Display a message indicating that there are no available flights for the selected date.            |
| Past Departure Date     | Select a past departure date                     | Display an error message indicating that the selected departure date is in the past.               |
| Future Departure Date   | Select a future departure date                   | Display available flight from Chicago to San Francisco on the specified future date.               |
| Empty Departure City    | Leave the departure city field empty             | Highlight the departure city field as required and prompt the user to enter a departure city.      |
| Empty Destination City  | Leave the destination city field empty           | Highlight the destination city field as required and prompt the user to enter a destination city.  |
| Empty Departure Date    | Leave the departure date field empty             | Highlight the departure date field as required and prompt the user to select a departure date.     |

