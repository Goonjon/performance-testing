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
<img width="459" alt="Screenshot 2024-09-16 122613" src="https://github.com/user-attachments/assets/70331cb6-7579-4d12-beb0-78a7652484cf">
<img width="761" alt="load-test-summary-report-of-booking" src="https://github.com/user-attachments/assets/a0dd867a-d93f-4095-9104-0f3398894d6a">
<img width="759" alt="load-test-statistics-of-boking" src="https://github.com/user-attachments/assets/041cb435-8ff9-4e17-a4e1-8b2bc075be19">


## Stress Test Report: (Booking)
<img width="573" alt="Screenshot 2024-09-15 225829" src="https://github.com/user-attachments/assets/79a8fa5a-ddb1-4043-9916-ff8203d37808">
<img width="764" alt="Screenshot 2024-09-16 014951" src="https://github.com/user-attachments/assets/5cf62531-ee0c-49fe-9132-282869a94233">
<img width="762" alt="Screenshot 2024-09-16 015021" src="https://github.com/user-attachments/assets/ae1c376b-dd28-4766-a06f-d6bccc0d9be6">

## Test Report: (dmoney)
<img width="761" alt="Summary-report-of-dmoney" src="https://github.com/user-attachments/assets/e7ca1f5a-19d1-47c6-ad07-fe2dfcf42531">
<img width="761" alt="Statistics-of-dmoney" src="https://github.com/user-attachments/assets/cb175676-9d97-4b85-8fa2-e00bfe51eb3c">
