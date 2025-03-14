# Performance Testing Report

## Performance Testing Screenshots

### `/all-student-name`
![Performance Test](https://github.com/user-attachments/assets/94c46f49-5eb3-4a44-bde2-1aa9c64a8a8c)

### `/highest-gpa`
![Performance Test](https://github.com/user-attachments/assets/03116eb4-d2f6-43d7-87f6-9016abb4b603)

## Test Plans

### `/all-student-name`
![Test Plan](https://github.com/user-attachments/assets/65668b30-a2ec-46e0-a615-cb4cd2cfbcd1)

### `/highest-gpa`
![Test Plan](https://github.com/user-attachments/assets/41dda9a6-5630-45f1-82fc-bf5a4b737508)

## Performance Testing Results

### Test Plan 1: `/all-student` (Optimization of `getAllStudentsWithCourses()`)

#### Before Optimization
- **JMeter GUI**
  ![Before Optimization](https://github.com/user-attachments/assets/80d2b28b-3711-4d65-b3b6-dda631ce5b32)
- **Command Line**
  ![Before Optimization](https://github.com/user-attachments/assets/1a006634-641d-42f5-b0b2-253108f8477f)

#### After Optimization
- **JMeter GUI**
  ![After Optimization](https://github.com/user-attachments/assets/1ee1e26a-d65c-4fb9-80eb-69ea4a303536)
- **Command Line**
  ![After Optimization](https://github.com/user-attachments/assets/0d8da548-86ef-48f6-8464-e4b50e379ab7)

### Test Plan 2: `/all-student-name` (Optimization of `jointStudentNames()`)

#### Before Optimization
- **JMeter GUI**
  ![Before Optimization](https://github.com/user-attachments/assets/e7753aa2-5858-4e94-883e-5d13534d3664)
- **Command Line**
  ![Before Optimization](https://github.com/user-attachments/assets/116d4f8a-1d50-421a-a417-b735d0db13b6)

#### After Optimization
- **JMeter GUI**
  ![After Optimization](https://github.com/user-attachments/assets/a4e10faa-a630-4c97-8658-352cde91f30c)
- **Command Line**
  ![After Optimization](https://github.com/user-attachments/assets/f528d6d2-2617-466f-a46b-f2e6e2081826)

### Test Plan 3: `/highest-gpa` (Optimization of `findStudentWithHighestGpa()`)

#### Before Optimization
- **JMeter GUI**
  ![Before Optimization](https://github.com/user-attachments/assets/880daa20-40cd-44b8-8d77-fef7d11bc74d)
- **Command Line**
  ![Before Optimization](https://github.com/user-attachments/assets/64660cd9-a88f-4fb7-8a11-9cac3fad9802)

#### After Optimization
- **JMeter GUI**
  ![After Optimization](https://github.com/user-attachments/assets/aaa4a250-e201-4a90-b483-577e2a1b390f)
- **Command Line**
  ![After Optimization](https://github.com/user-attachments/assets/ec30dea6-7a93-488b-8331-fdb11d74072e)

## Questions & Answers

### 1. Difference Between JMeter and IntelliJ Profiler for Performance Testing
JMeter is a load and performance testing tool that simulates user interactions with an application to measure system-wide performance under various conditions. It helps identify high-level performance issues such as slow database queries, CPU/memory usage spikes, and network latency.

IntelliJ Profiler, on the other hand, provides a detailed analysis of an application's runtime behavior, helping developers pinpoint inefficient code, memory leaks, excessive garbage collection, and slow method executions. While JMeter detects system-level issues, IntelliJ Profiler provides in-depth code-level insights for optimization.

### 2. How Profiling Helps Identify Weak Points in an Application
Profiling helps by:
- Providing detailed insights into CPU usage, memory consumption, and method execution times.
- Highlighting methods consuming excessive resources.
- Detecting memory leaks and inefficient garbage collection.
- Pinpointing slow method calls and high CPU/memory usage.

### 3. Effectiveness of IntelliJ Profiler in Identifying Bottlenecks
Yes, IntelliJ Profiler is highly effective. It offers:
- Real-time analysis of CPU, memory, and thread activity.
- Flame graphs and call trees to visualize performance bottlenecks.
- Insights into method execution times, helping developers optimize critical functions.

### 4. Challenges in Performance Testing & Profiling
#### Challenges:
1. Deciding how to optimize inefficient code.
2. Identifying whether bottlenecks stem from code, database, or external factors.
3. Understanding JMeter and profiling tools.

#### Solutions:
- Analyzing execution traces and logs to pinpoint bottlenecks.
- Using profiling tools alongside JMeter to correlate findings.
- Continuous learning and practice to improve proficiency.

### 5. Benefits of Using IntelliJ Profiler
1. **Detailed Code-Level Insights** - Visibility into CPU, memory, and execution times.
2. **Detection of Performance Bottlenecks** - Identifies slow-performing methods.
3. **Flame Graphs & Call Trees** - Helps visualize code execution and optimization areas.

### 6. Handling Inconsistencies Between JMeter and IntelliJ Profiler Results
1. **Analyze the Bottleneck** - Determine if it's system-level (JMeter) or code-level (Profiler).
2. **Reproduce and Isolate Issues** - Run profiling during JMeter load tests to correlate findings.

### 7. Optimization Strategies Based on Testing & Profiling Results
1. **Optimize Hotspots** - Refactor slow-performing methods.
2. **Enhance Database Performance** - Optimize queries, indexing, and caching.
3. **Implement Efficient Algorithms** - Reduce redundant computations and optimize loops.

