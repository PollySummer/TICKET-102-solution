# TICKET-102 solution

To solve this task, I:
1) created a CheckAge method that first extracts the first 6 digits of the personal code; 
2) divided the extracted digits into year, month and day, and then converted them into a format convenient for comparison; 
3) In part: \
   <i>if (year >= 22) { \
   year += 1900; \
   } else { \
   year += 2000; \
   }</i> \
   I'm checking the first two digits to determine the century in which the person was born;
   (since I originally had a bug that for people born in the 1900s, it said they were under 18). 
4) Find out the client's age using dateOfBirth and compare it to the currentDate. 
5) Return a boolean value indicating whether the client's age meets the criteria for credit approval. 
   In this way, every day the information about the clients who can take a loan will change.