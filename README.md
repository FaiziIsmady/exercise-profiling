Performance testing screenshot for /all-student-name and /highest-gpa.

`/all-student-name`
![Image](https://github.com/user-attachments/assets/94c46f49-5eb3-4a44-bde2-1aa9c64a8a8c)

`/highest-gpa`
![Image](https://github.com/user-attachments/assets/03116eb4-d2f6-43d7-87f6-9016abb4b603)

Test plans that previously created for endpoint /all-student-name and /highest-gpa via command line

`/all-student-name`
![Image](https://github.com/user-attachments/assets/65668b30-a2ec-46e0-a615-cb4cd2cfbcd1)

`/highest-gpa`
![Image](https://github.com/user-attachments/assets/41dda9a6-5630-45f1-82fc-bf5a4b737508)

Performance test on file `test_plan_1` `/all-student` based on `getAllStudentsWithCourses()` optimization

Before `getAllStudentsWithCourses()` optimization
jmeter GUI
![Image](https://github.com/user-attachments/assets/80d2b28b-3711-4d65-b3b6-dda631ce5b32)

via Command Line
![Image](https://github.com/user-attachments/assets/1a006634-641d-42f5-b0b2-253108f8477f)

After `getAllStudentsWithCourses()` optimization
jmeter GUI
![Image](https://github.com/user-attachments/assets/1ee1e26a-d65c-4fb9-80eb-69ea4a303536)

via Command Line
![Image](https://github.com/user-attachments/assets/0d8da548-86ef-48f6-8464-e4b50e379ab7)

Performance test on file `test_plan_2` `/all-student-name` based on `jointStudentNames()` optimization<br>
Before `jointStudentNames()` optimization
jmeter GUI
![Image](https://github.com/user-attachments/assets/e7753aa2-5858-4e94-883e-5d13534d3664)

via Command Line
![Image](https://github.com/user-attachments/assets/116d4f8a-1d50-421a-a417-b735d0db13b6)

After `jointStudentNames()` optimization
jmeter GUI
![Image](https://github.com/user-attachments/assets/a4e10faa-a630-4c97-8658-352cde91f30c)

via Command Line
![Image](https://github.com/user-attachments/assets/f528d6d2-2617-466f-a46b-f2e6e2081826)

Performance test on file `test_plan_3` `/highest-gpa` based on `findStudentWithHighestGpa()` optimization<br>
Before `findStudentWithHighestGpa()` optimization
jmeter GUI
![Image](https://github.com/user-attachments/assets/880daa20-40cd-44b8-8d77-fef7d11bc74d)

via Command Line
![Image](https://github.com/user-attachments/assets/64660cd9-a88f-4fb7-8a11-9cac3fad9802)

After `findStudentWithHighestGpa()` optimization
jmeter GUI
![Image](https://github.com/user-attachments/assets/aaa4a250-e201-4a90-b483-577e2a1b390f)

via Command Line
![Image](https://github.com/user-attachments/assets/ec30dea6-7a93-488b-8331-fdb11d74072e)

Please answer the following questions:
1. What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance? <br>

JMeter is primarily used for load testing, stress testing, and performance benchmarking at the system level. It simulates multiple users interacting with the application to measure response times, throughput, error rates, and resource utilization under various load conditions. <br> 
This helps identify bottlenecks such as slow database queries, high memory or CPU usage, and network latency issues. It is typically used in pre-production or staging environments to ensure scalability and stability under real-world conditions. <br>
In contrast, IntelliJ Profiler is used for deep code-level analysis, providing insights into CPU usage, memory allocation, garbage collection, and method execution times. It helps developers pinpoint inefficient code, memory leaks, excessive garbage collection, and slow method calls using flame charts and call graphs. <br>
The profiler is usually applied in development or debugging environments to fine-tune code efficiency. While JMeter helps detect high-level system performance issues, IntelliJ Profiler enables detailed analysis and optimization at the code level.

2. How does the profiling process help you in identifying and understanding the weak points in your application? <br>

The profiling process helps identify and understand weak points in an application by providing detailed insights into its runtime behavior, <br>
including CPU usage, memory consumption, thread activity, and method execution times. By using a profiler such as IntelliJ Profiler, <br>
developers can analyze performance bottlenecks at a granular level. It highlights which methods or functions consume the most CPU, take excessive execution time, or cause frequent context switches. <br>
Additionally, memory profiling helps detect memory leaks, excessive object creation, and inefficient garbage collection patterns that may lead to high memory usage or application slowdowns.

3. Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code? <br>

Yes, IntelliJ Profiler is highly effective in analyzing and identifying bottlenecks in application code. It provides real-time insights into CPU usage, memory allocation, garbage collection, <br>
and thread activity, helping developers pinpoint inefficiencies at a granular level. The call tree and flame graph visualizations make it easy to see which methods consume the most resources, allowing for targeted optimizations.

4. What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges? <br>

There are several challenges I found:<br>

4.1 Deciding on what to do on uneficient code<br>

4.2 Determining if it is my code that is inneficient or other causes (bottleneck identification)<br>

4.3 Trying to understand jmeter and profiling

5. What are the main benefits you gain from using IntelliJ Profiler for profiling your application code? <br>

5.1 Detailed Code-Level Insights<br>
IntelliJ Profiler provides granular visibility into CPU usage, memory allocation, method execution times, and thread activity.<br>

5.2 Detection of Performance Bottlenecks<br>
Profiler highlights hotspots—methods that consume the most CPU or take the longest to execute.<br>

5.3  Flame Graphs and Call Trees for Better Visualization <br>
The profiler generates flame graphs, call trees, and execution timelines, making it easier to visualize how the application executes and where optimizations are needed.<br>

6. How do you handle situations where the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter? <br>

6.1 Analyze Bottleneck<br>
JMeter tests system-wide performance (network, database, server load), while IntelliJ Profiler focuses on code-level inefficiencies. Identify if the issue is at the application level (CPU, memory leaks) or system level (latency, database, API performance).

6.2 Reproduce and Isolate Issues<br>
Run profiling during a JMeter load test to observe application behavior under actual load, helping correlate findings between both tools.

7. What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?<br>

7.1 Optimize Hotspots<br>
Refactor or optimize methods consuming excessive CPU, memory, or execution time.<br>

7.2 Enhance Database Performance<br>
Optimize queries, add indexing, use caching, and reduce unnecessary database calls.<br>

7.3 Implement Efficient Algorithms<br>
Replace inefficient loops, recursive calls, and redundant computations with optimized alternatives.<br>



