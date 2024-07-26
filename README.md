README
Automation QA Home Assignment
Setup
Environment Setup
1.	Install Node.js:
o	Ensure Node.js is installed. If not, download and install it from Node.js official website.
2.	Install Playwright:
o	Run the following command in your terminal to install Playwright:
npm init playwright@latest
o	Follow the prompts to set up the project.
3.	Install Dependencies:
o	Navigate to your project directory and install necessary packages:
npm install
WebDriver Setup
•	Playwright comes with its own drivers, so no additional WebDriver setup is needed.
Test Plan
App/Homepage Load
1.	Verify Homepage Load:
o	Ensure the homepage loads successfully.
o	Check the presence of key elements like buttons, language selector, and main sections.
Navigation
1.	Verify Navigation Links:
o	Ensure all links in the navigation bar lead to the correct pages.
2.	Browser Navigation:
o	Verify the back and forward buttons in the browser work as expected.
Room Upgrades and Product Listings
1.	Verify Display:
o	Ensure room upgrades and product listings are displayed correctly.
o	Verify each offer includes necessary information such as name, price, and description.
Reporting
•	Generate Report:
o	Generate a report of executed test cases indicating the pass/fail status.
o	Provide screenshots for failed tests to indicate the issues.
Instructions to Run Tests
1.	Navigate to Project Directory:
cd your-project-directory
2.	Run Tests:
o	Execute the test cases:
npx playwright test
3.	Generate Report:
o	View the test report:
npx playwright show-report

Assumptions
•	The application URL is correctly configured in the test scripts.
•	All necessary elements have unique and identifiable selectors.
Thought Process and Approach
1.	Homepage Load:
o	Focused on essential elements that indicate a successful load.
2.	Navigation:
o	Ensured that all navigation links are functional and lead to the correct pages.
3.	Room Upgrades and Product Listings:
o	Verify that all product listings are displayed correctly with detailed information.
4.	Surprise Us:
o	Tested the login feature in the webpage
o	Tested the language drop down in the webpage
o	The locators are stored in a separate utility class to increase the readability and reusability.
o	End to end test to track the product details from homepage to the confirmation page
5.	Reporting:
o	Implement detailed reporting with screenshots to facilitate debugging.
6.	Additional Scope
o	Slider Functionality for Placing Bids:
•	Test the slider used for placing bids, ensuring it works correctly within the end-to-end workflow. Verify that the product summary and price on the confirmation page are accurate.
o	Points-Based Purchases:
•	Ensure that signed-in users can use their points to purchase products. Test this functionality thoroughly.
o	Dynamic Page Testing:
•	Utilize Playwright's built-in features to test the dynamic nature of the page, ensuring all dynamic elements behave as expected.

Detailed description:
You can execute individual tests located in the "tests" folder by using the command: `npx playwright test`. For example, to run the "language selector.spec.js" test, please use the following command: `npx playwright test tests/languageselector.spec.js --headed`. After running the test, you can view the reports by using the command `npx playwright show-report`. These commands should be entered in the terminal. The report will automatically appear after executing the command, or alternatively, you can access the report on your localhost. The report includes screenshots and even video recordings. Additionally, Allure reporting can be seamlessly integrated into the framework, providing more detailed and visually appealing insights.




