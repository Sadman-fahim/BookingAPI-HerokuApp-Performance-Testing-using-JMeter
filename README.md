# BookingAPI (HerokuApp) Performance Testing using JMeter

Scripts and reports for performance testing the BookingAPI on HerokuApp are available in this repository. The system's ability to manage multiple concurrent requests and monitor its performance under various loads was assessed using Apache JMeter, a well-known open-source load testing tool.

## Overview

The purpose of the BookingAPI test site is to mimic a booking API. It functions as a platform for evaluating and verifying how well systems communicate with a booking API. The base URL is [https://restful-booker.herokuapp.com](https://restful-booker.herokuapp.com), providing endpoints for scheduling, availability checking, and other associated tasks.

## Test Setup

Performance testing with varying concurrency levels was carried out using JMeter. Each test measured the system's error rate, throughput, and response time by executing a predetermined number of concurrent requests with a defined loop count.

### Tests Conducted:

1. **100 Concurrent Requests with 10 Loop Count**
   - Average Transactions Per Second (TPS): ~88
   - Total Concurrent API Requests: 600

2. **200 Concurrent Requests with 10 Loop Count**
   - Average TPS: ~92
   - Total Concurrent API Requests: 1200

3. **300 Concurrent Requests with 10 Loop Count**
   - Average TPS: ~146
   - Total Concurrent API Requests: 1800

4. **500 Concurrent Requests with 10 Loop Count**
   - Average TPS: ~223
   - Total Concurrent API Requests: 3000

5. **800 Concurrent Requests with 10 Loop Count**
   - Average TPS: ~276
   - Total Concurrent API Requests: 4800

6. **1200 Concurrent Requests with 10 Loop Count**
   - Average TPS: ~399
   - Total Concurrent API Requests: 7200

7. **1500 Concurrent Requests with 10 Loop Count**
   - Average TPS: ~46
   - Total Concurrent API Requests: 9000  
   - Error Rate: 0.20% (18 connection timeouts)

8. **2000 Concurrent Requests with 10 Loop Count**
   - Average TPS: ~280
   - Total Concurrent API Requests: 12000

## Test Results

The performance testing results indicate that the BookingAPI on HerokuApp can manage up to **42,000 concurrent requests** with an error rate near zero. The tests demonstrated the system's resilience and capacity to handle a significant volume of requests while maintaining respectable throughput and response times.

### Detailed Reports

- [100 Concurrent Requests Report](#)
- [200 Concurrent Requests Report](#)
- [300 Concurrent Requests Report](#)
- [500 Concurrent Requests Report](#)
- [800 Concurrent Requests Report](#)
- [1200 Concurrent Requests Report](#)
- [1500 Concurrent Requests Report](#)
- [2000 Concurrent Requests Report](#)

## Conclusion

The BookingAPI on HerokuApp exhibits robust performance characteristics, showcasing impressive scalability by handling tens of thousands of concurrent API requests with negligible error rates.

## Contributing

Contributions are welcome! If you have improvements to the existing tests or want to contribute new ones, feel free to open an issue or submit a pull request. Your contributions will help enrich this repository and enhance the understanding of application performance through detailed analysis.

## Frequently Asked Questions (FAQs)

### Q1: What is the purpose of this repository?

This repository documents performance testing conducted on the BookingAPI on HerokuApp using JMeter. It includes test plans, results, and generated reports for various concurrency levels.

### Q2: What is the BookingAPI on HerokuApp?

The BookingAPI on HerokuApp is a test platform that simulates a booking API, providing endpoints for creating, updating, or deleting bookings, among other functionalities.

### Q3: Why was JMeter used for performance testing?

JMeter is an open-source tool for load, performance, and stress testing. It allows testers to simulate various scenarios, measure response times, and analyze performance under different loads.

### Q4: How were the performance tests conducted?

Tests were executed using a series of concurrent requests with fixed loop counts. Metrics such as response time, throughput, and error rates were measured to evaluate system performance.

### Q5: What were the key findings from the tests?

The BookingAPI can handle up to 42,000 concurrent requests with minimal error rates, demonstrating scalability and stability.

### Q6: How can I contribute?

Fork this repository, make your changes, and submit a pull request. Contributions that align with the project scope are welcome!

---

Feel free to explore and use the test results for reference in your performance testing projects!

