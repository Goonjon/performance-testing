# Performance Testing with Jmeter
### Project Summary: This project focuses on performance testing for two distinct scenarios:
### 1. Booking System Load and Stress Testing: Simulating 120,000 users over a 12-hour period logging in, creating bookings, and searching for bookings.
### 2. Dmoney API JMeter Testing: Involving deposits, money transfers, payments, and withdrawals using agents, customers, and merchants, with Boundary Value Analysis (BVA) applied to withdrawal amounts.

## Technologies I have used: 
- JMeter
- Java
- Postman: For API testing and generating the base test collections

## How to run?
Scenario 1: Booking System Load and Stress Testing
1. Open Apache JMeter from command prompt directly or open from the bin folder as jar file.
2. Ensure JMeter is configured properly.
3. Open the booking.jmx file in JMeter.
4. Set up threads collection with necessary files.

Load Test:
1. Set the number of users and ramp-up time according to your needs.
2. Limit the load test duration to 20 minutes for faster testing.
3. Run the test and view reports.

Stress Test:
1. After a successful load test, gradually increase users to find the bottleneck.

Scenario 2: Dmoney API JMeter Testing
1. Open the bin folder and set up CSV files: `deposit.csv`, `sendMoney.csv`, `payment.csv`, `withdraw.csv`.
2. Open `dmoney.jmx` in JMeter.
3. Set the appropriate ramp-up time (120 secs).
4. For each transaction type (deposit, sendMoney, payment, withdrawal), configure the threads.
5. Run the test and view reports.


## How to create manual report?
1. Open the `.jmx` file in JMeter.
2. Run the test manually within JMeter.
3. Record the load test and stress test results.
4. Add the recorded data into an Excel sheet to create a manual report.

## How to generate html report?
1. After the test, navigate to the test folder and open a command prompt.
2. Run the command to generate the HTML report ```jmeter -n -t your_test.jmx -l your_test.jtl -e -o Reports```
3. Open the `Reports` folder to view the HTML report.

## Load Test Report: (Booking)
<img width="459" alt="Screenshot 2024-09-16 122613" src="https://github.com/user-attachments/assets/22519ebe-e445-4588-8c3b-cf424938cb98">
<img width="761" alt="load-test-summary-report-of-booking" src="https://github.com/user-attachments/assets/b1f59670-1ac3-414b-85a7-e5e901404501">
<img width="759" alt="load-test-statistics-of-boking" src="https://github.com/user-attachments/assets/f0086a3f-5d90-4911-8936-23c5b505d045">

## Stress Test Report: (Booking)
<img width="573" alt="Screenshot 2024-09-15 225829" src="https://github.com/user-attachments/assets/e1ebba3b-db75-4f09-9711-55646edd2009">
<img width="764" alt="Screenshot 2024-09-16 014951" src="https://github.com/user-attachments/assets/8a0871ee-dc9a-4e76-9d86-f1640ee4a2f3">
<img width="762" alt="Screenshot 2024-09-16 015021" src="https://github.com/user-attachments/assets/f91e7ace-23d1-4121-bfa7-990d6172e5f9">

## Test Report: (dmoney)
<img width="761" alt="Summary-report-of-dmoney" src="https://github.com/user-attachments/assets/9453dbb6-81ab-4ead-882b-13ba9444df09">
<img width="761" alt="Statistics-of-dmoney" src="https://github.com/user-attachments/assets/36ff7578-9697-4089-8614-0610aae799d1">
