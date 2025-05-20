```Problem Statement```
A school is preparing a trip for 400 students. The transportation company has 10 buses of 50 seats each and 8 buses of 40 seats but only has 9 drivers available.
The rental cost for a large bus is 800 and 600 for a small bus. 
Calculate how many buses of each type should be used for the trip for the least possible cost. 

Steps to Solve
We'll define:
• Decision variables:
Let x be the number of large buses used
Let y be the number of small buses used
• Objective:
Minimize 800x + 600y
• Subject to constraints:
o 50x + 40y >= 400 (enough seats)
o x <= 10 (max 10 large buses)
o y <= 8 (max 8 small buses)
o x + y <= 9 (max 9 drivers)
o x, y are integers ≥ 0
