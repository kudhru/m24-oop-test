**Cricket Analytics Application** [Total Marks: 35, Approximate Time: 1 hour 15 minutes]

You are required to implement functionalities for a Cricket Analytics application. The provided template code for this application contains multiple classes and methods related to cricket players, their roles, team information, and various data-handling operations. Your tasks involve implementing several methods, each responsible for performing specific actions like reading data from a file, writing data back, updating player statistics, and filtering data.

You are strictly required to use and stick to the template code provided to you and implement the parts marked with questions. You have been provided with the following files for this question:

1. **CricketAnalytics.java** [Code template file where you need to write code for this question]
2. **inputCricketData.csv** [Input file which is required to be read as part of this question]

### **Tasks and Methods to be Implemented**

For each method, use the provided comments as a guide for implementation. Follow the instructions to complete the methods. Only when explicitly mentioned, please handle errors and/or raise exceptions. **You are neither allowed to change the signature of any method nor you are allowed to add any member variables in any class. You just need to write code within the mentioned methods.**

#### 1. **RunsComparator: compare Method [2 marks]**

- **Location:** `RunsComparator` class
- **Task:** Write code for comparing runs scored by two players in descending order.
  - Return a negative value if the first player has more runs, a positive value if the second player has more runs, or zero if they have the same number of runs.

#### 2. **CricketDataHandler: readPlayersFromFile Method [9 marks]**

- **Location:** `CricketDataHandler` class
- **Task:** Write code for reading player data from the input CSV file and creating a list of `Player` objects.
  - Step 1: Create an empty list to store player details. [1 mark]
  - Step 2: Open the specified file for reading data. [1 mark]
  - Step 3: Ignore the first line since it contains the column names. [1 mark]
  - Step 4: Read each line one by one until reaching the end of the file. [1 mark]
  - Step 5: Split the line into different pieces of information. [1 mark]
  - Step 6: Create a new player using this information. [1 mark]
  - Step 7: Add the new player to the list. [1 mark]
  - Step 8: Close the file after reading all data. [1 mark]
  - Step 9: Return the complete list of players. [1 mark]

#### 3. **CricketDataHandler: writePlayersToFile Method [4 marks]**

- **Location:** `CricketDataHandler` class
- **Task:** Write code to write the updated list of players back to the output CSV file. The format of the output file should be the same as that of the input file.
  - Step 1: Prepare to write data into the specified file. [1 mark]
  - Step 2: Write the column names as the first line of the file. [1 mark]
  - Step 3: For each player in the list, convert their details to the desired format. [1 mark]
  - Step 4: Write each player's information to the file. [1 mark]

#### 4. **CricketDataHandler: updatePlayerStats Method [5 marks]**

- **Location:** `CricketDataHandler` class
- **Task:** Implement the method to update a player's stats (runs and wickets).
  - Step 1: Go through each player in the list. [1 mark]
  - Step 2: Check if the current player's name matches the given name. [1 mark]
  - Step 3: If it matches, update the player's runs with the new value. Updated value will be the sum of the old runs and the argument runs. For example, if a player had 100 runs and the runs argument (to this method) is 50, their new total should be 150 runs. [1 mark]
  - Step 4: Similarly, update the player's wickets with the new value. Updated value will be the sum of the old wickets and the argument wickets. For example, if they had 10 wickets and the wickets argument (to this method) is 2, their new total should be 12 wickets[1 mark]
  - Step 5: If no player matches the given name, throw an IllegalArgumentException exception. [1 mark]

#### 5. **CricketDataHandler: calculateTeamAverageRuns Method [5 marks]**

- **Location:** `CricketDataHandler` class
- **Task:** Write code to calculate the average runs scored by players of a specific team.
  - Step 1: Filter players belonging to the specified team. [2 marks]
  - Step 2: If no players from the specified team are found, throw an IllegalArgumentException exception. [1 mark]
  - Step 3: Calculate the total runs scored by all players from this team. [1 mark]
  - Step 4: Compute and return the average runs scored. [1 mark]

#### 6. **TeamFilterStrategy: filter Method [5 marks]**

- **Location:** `TeamFilterStrategy` class
- **Task:** Write code to filter players by their team.
  - Step 1: Create an empty list for players matching the criteria. [1 mark]
  - Step 2: Go through each player in the players list. [1 mark]
  - Step 3: If the player's team matches the given name, add them to the list. [2 marks]
  - Step 4: Return the list containing all matching players. [1 mark]

#### 7. **AllRounderStatsFilter: filter Method [5 marks]**

- **Location:** `AllRounderStatsFilter` class
- **Task:** Write code to filter all-rounder players which satisfy the provided criteria (i.e. filter those all-rounders who have runs and wickets greater than or equal to the runs and wickets specified in the criteria respectively).
  - Step 1: Create an empty list for players matching the criteria. [1 mark]
  - Step 2: Go through each player in the list. [1 mark]
  - Step 3: If the player is an all-rounder and meets the given criteria for both runs and wickets, add them to the list. [2 marks]
  - Step 4: Return the list containing all matching players. [1 mark]

### **Instructions to Students**

1. Before starting to write the code, read the entire question and go through the entire question. This is a very simple question. Just take a deep breath and write code peacefully!
2. Write your implementation only in the designated areas marked by the questions and comments.
3. Do not modify any parts of the code not mentioned in the questions.
4. Do not change the names and signatures of the methods.
5. Do not add any member variables in any class.
6. Before submission, run your implementation to ensure that your code compiles successfully.
