# PolyU AAE1001 GitHub Project Group 13

# Members 
Leader: Law Yat Hei Daniel

Member 1: Lau Pak Kuai Enrico

Member 2: Zhou Jian Hong

Member 3: Zhang Ding Zhe

Member 4: Sun Chu Rui

Member 5: Ng Tsz Hin

Member 6: Sun Xiao

Member 7: Shek Pui Ka Hannah

## Table of Contents
- [Introduction](#introduction)
- [Tasks](#tasks)
  - [Task 1](#task-1)
  - [Task 2](#task-2)
  - [Task 3](#task-3)
- [Reflections](#reflections)
- [Contacts](#contacts)

## Introduction
This project focuses on optimizing airline operations by minimizing costs and maximizing efficiency through strategic pathfinding and aircraft selection. The project is divided into three tasks, each addressing different scenarios and challenges.

## Tasks

### Task 1
**Objective:** Identify the most cost-effective aircraft for different scenarios.

**Approach:** Some areas the flight route may encounter may cost extra fuel or time.In order to minimalise the cost, flight planning will consider factors like fuel costs, time-related costs, and operational constraints. After obtaining the flight route with lowest cost,the data obtained will be used to select the best aircraft model.

For flight path planning, we first set up the obstacle map, the start and the end position of the route.

![image](https://github.com/user-attachments/assets/8df7fa77-2c05-4a79-a238-4038be83e861)
![image](https://github.com/user-attachments/assets/0dd8d4e5-f3ae-4d12-8d2f-c2972369b83b)

Then, we set up the cost intensive area (fuel intensive, time intensive).

![image](https://github.com/user-attachments/assets/2a4df736-a152-4665-a5c3-696d0bb00a67)

After that, we set the cost value of the area.

![image](https://github.com/user-attachments/assets/e3b2a15e-837a-48a9-b701-fd49a64d4076)

Finally, the route can be found.

![image](https://github.com/user-attachments/assets/8620336f-fcfa-448d-b81c-48411efa0b2f)

Then, by calculation, we can find the aircraft type most suitable for the route for different simulation.

![image](https://github.com/user-attachments/assets/0d8e738d-5888-41d5-8a1a-da74d1f5aeee)



### Task 2
**Goal:** Design a new cost area that can reduce the cost of the route by leveraging jet streams.

**Methodology:** Introduce a jet stream area to reduce flight time and fuel consumption, achieving significant cost savings. When aircraft is flying along jet stream, the resultant drag exerted on the aircraft by air is smaller. Thus the efficiency of the engine will increase and have a lower cost to travel the same distance.

First, the area of the jet stream is set.

![image](https://github.com/user-attachments/assets/e4580f58-c4df-4eb0-ac22-1c28ed455f73)

Then, the cost modifier of the jet stream area is set.

![image](https://github.com/user-attachments/assets/dd46a5f8-3295-44c1-b2ea-12108462a1e1)
![image](https://github.com/user-attachments/assets/5a804a94-d9b1-4841-86a1-67470c94f562)

Finally, the jet stream can be plotted and the new route can be found.

![image](https://github.com/user-attachments/assets/e78cf1ee-0e19-4668-aebf-273ef2970091)

This is the cost, and the previous cost

![image](https://github.com/user-attachments/assets/838244b4-d6da-4b5b-bb4f-9f22c9ac8dd4)
![image](https://github.com/user-attachments/assets/3a7baa41-b4dc-42d5-ae90-a6022ab16e45)



### Task 3
**Introduction:**
This project provides a deep analysis of the operational costs associated with different aircraft designs based on passenger capacity. It utilizes Python and Matplotlib to visualize the cost comparison and optimal design for an aircraft that can accommodate a total of 3,000 passengers across multiple flights.


**Specifications:**
- Calculates the optimal aircraft design based on various parameters such as passenger capacity, number of engines, and associated costs.
![屏幕截图 2024-11-12 133017](https://github.com/user-attachments/assets/f8c2ca1f-afbe-4303-b166-8c17e7155896)
- Visualizes the total operating costs for different aircraft capacities using bar charts.
![屏幕截图 2024-11-12 133228](https://github.com/user-attachments/assets/85452614-de08-4e98-802a-77eca257b2cd)
- Analyzes the composition of costs (fuel, time, fixed costs) using pie charts.
![屏幕截图 2024-11-12 133305](https://github.com/user-attachments/assets/740af5b4-fe36-45f8-a08c-6807b0dd96a7)
- We can find minimum cost of the most suitable aircraft, and design both bar chart and pie chart.
![屏幕截图 2024-11-12 134555](https://github.com/user-attachments/assets/052a08c5-7917-48ef-8269-43952528544c)


**Detailed Calculation:** Calculate operational costs for different passenger capacities to determine the most cost-effective configuration.



## Additional Tasks

###Additional Task 3
**Objective:** 
Compare Dijkstra Path Planning, A* Path Planning and Greedy Best First Search path planning algorithm.

**Details:** 
Before starting, it is important to understand the mechanism of the three algorithms

A*:
Searches the map starting from the start node, prioritizing nodes in the direction towards goal node from the node at that instant, backtracks when encountered an obstacle and start searching for the next closest node.

Dijkstra:
Similar to A*, however, it does not prioritize on searching the nodes closer to the goal node, instead it progressively searches the whole map until it reaches the goal node.
Dijkstra can be described as a more "blind" version of A*.

Greedy Best first Search:
From the start node, go towards the direction of the goal node, when encountered an obstacle, start a Dijkstra's search until it can go around the obstacle, then repeat.

**Approach:** 
For an effective comparison, all 3 algorithms should use the same map.
The design of the map is as follow:
![Screenshot 2024-11-15 174209](https://github.com/user-attachments/assets/0b44cee4-f990-448d-947d-1ba1078931b9)

**Path from Algorithms:**
The path obtained from the algorithms are as follow:

A*:

![Screenshot 2024-11-15 173947](https://github.com/user-attachments/assets/62a28879-c7b3-403d-b11a-0236d6cfb34b)

Dijkstra:

![Screenshot 2024-11-15 174015](https://github.com/user-attachments/assets/bbc71e2c-6b59-4ed1-89d3-3175e6b7386b)

Greedy Best First Search:

![Screenshot 2024-11-15 173921](https://github.com/user-attachments/assets/e8d2cfc9-1c14-4e14-b63d-5645505cd0a5)

**Comparison:**

After analyzing the path results, a comparison is made.

Algorithms | A* | Dijkstra | Greedy Best First Search
Search Speed | Moderate | Slow | Fast
Shortest path | Yes | Yes | No

By analyzing the algorithms, some potential advantages of the three algorithms are found.

A*
- generally a better, less process intensive version of Dijkstra
- more efficient than Dijkstra in longer paths

Dijkstra
- does not rely on path cost
- guaranteed to find the shortest path

Greedy Best First Search
- less process intensive
- can find path in less time

Here are some potential applications of the three algorithms.

A*
- finding optimal path in well-defined areas with lighter processing load

Dijkstra
- finding optimal path in poorly-defined areas with a higher processing load

Greedy Best First Search
- finding a path to goal in a short time with little processing load



## Reflections

Group Leader, Daniel Law Yat Hei

As a gruop leader, I find myself trapped within the burden of leading the team, dealing with unfamiliar task and the immense workload of other subjects
It is undoubtedly impossible for me to finish the project alone. However, thanks to my groupmates, we're able to complete the task we're assigned.
It may not be perfect, but this is indeed the hard work of the team. Other than trying to program with python for the fisrt time, I've learned that one can only walk so far without a team.
Also, I've benefit immensely from taking the leading role. I've understood the importance of time management. Since the presentation day 
is close to another midterm test, starting to work on the project early becomes critical to finishing the task in time.
Another thing is that benig a leader is not just assigning task to teamates, but also get down to the field and help them out,
while keeping an eye on the overview of the progress and keep track of it.

Group member, Zhou Jian Hong

This was my first time to learn programming. I was very confused at the beginning, but through constant exploration in the sample examples and the explanations from the team leader and team members, I gained a preliminary understanding of programming and participated in the project. This also made me realize the importance of teamwork. With the advice of teaching assistant and professor, I was able to do a better job in the project, which also aroused my interest in programming and benefited me a lot.

Group member, Zhang Dingzhe

As a group member, I gained a lot from this project. Our group leader allocated all the tasks reasonably, and Churui and I were assigned task 3. Throughout the project, our leader checked our progress in time to ensure the whole group's progress. I really benefit from cooperating with Churui, who is very inspiring. Communication, never neglect and learning all the time are important for group projects.

## Contacts
For more information, please contact the project leader or any of the team members.

Group leader, Daniel Law Yat Hei 24075347@connect.polyu.hk

Group member, Zhang Dingzhe 24111786d@connect.polyu.hk
