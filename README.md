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
**Name for our aircraft:** 

**Specifications:**
- Passenger capacity: 
- Engine count: 

**Detailed Calculation:** Calculate operational costs for different passenger capacities to determine the most cost-effective configuration.

## Reflections

Group Leader, Daniel Law Yat Hei
As a gruop leader, I find myself trapped within the burden of leading the team, dealing with unfamiliar task and the immense workload of other subjects
It is undoubtedly impossible for me to finish the project alone. However, thanks to my groupmates, we're able to complete the task we're assigned.
It may not be perfect, but this is indeed the hard work of the team. Other than trying to program with python for the fisrt time, I've learned that one can only walk so far without a team.
Also, I've benefit immensely from taking the leading role. I've understood the importance of time management. Since the presentation day 
is close to another midterm test, starting to work on the project early becomes critical to finishing the task in time.
Another thing is that benig a leader is not just assigning task to teamates, but also get down to the field and help them out,
while keeping an eye on the overview of the progress and keep track of it.

## Contacts
For more information, please contact the project leader or any of the team members.
