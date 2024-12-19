# NCAA 2023 Women's Volleyball Tournament  
## Clutch Players Analysis  

**Author**: Joshua Bastin  

## Introduction  

Each year, the **NCAA Women’s Volleyball Tournament** features **64 teams** competing in a **single-elimination, March Madness-style bracket** to determine the national champion. Teams qualify through **31 automatic conference championship bids** and at-large selections. Matches progress until one team is crowned **NCAA Champion**.  

### Key Rules of NCAA Volleyball  

To better understand the analysis, here are some **basic rules** of NCAA volleyball:  
- **Match Structure**: Matches are played as a **best of 5 sets**. The first team to win **3 sets** wins the match.  
- **Scoring a Set**: Each set is played to **25 points**, but a team must win by **2 points**. If tied, play continues until one team achieves a 2-point lead.  
- **Tiebreaker Set**: If teams split the first four sets (2-2), a deciding **5th set** is played to **15 points**, with teams switching sides when a team reaches **8 points**. The win-by-2 rule still applies.

---

## Purpose of the Project  

This project analyzes the **most clutch players** of the **2023 NCAA Women’s Volleyball Tournament**. Players are evaluated based on their performance during critical **"clutch" moments** of play, defined as occurring under **either** of the following conditions:  

1. **Score Conditions**:  
   - Both teams have reached **at least 17 points** in the set.  
   - The score differential is **±2 points**.  

**OR**  

2. **Tiebreaker Set**:  
   - The match is in the **5th or deciding set**.  

---

## Key Metrics Analyzed  

To identify standout performers in clutch time, the analysis focuses on **three primary point-scoring metrics**:  

1. **Attacking**  
2. **Serving**  
3. **Blocking**  

Each metric is carefully defined and measured using detailed **play-by-play data** from the tournament.

---

## Metric Descriptions  

### 1. Attacking  
Attacking occurs when a player attempts to **hit the ball to the opponent’s side** to score a point. The performance metric used to evaluate the most clutch attackers is **hitting efficiency**, calculated as:  

$\frac{\text{Kills} - \text{Errors}}{\text{Total Attempts}}$

- **Kill**: A successful attack that scores a point.  
- **Error**: An unforced mistake, such as hitting the ball into the net or out of bounds.  
- **Attempt**: Each time the player attempts to hit the ball.  

**Example**:  
A player has **5 kills**, **2 errors**, and **10 total attempts**.  

$\text{Hitting Efficiency} = \frac{5 - 2}{10} = 0.300$

A hitting efficiency of **0.300 or higher** is generally considered **good**, though this can vary depending on the player's position.

---

### 2. Serving  
Serving is the act of starting a rally by hitting the ball over the net to the opponent’s side. The key metric for evaluating clutch servers is **aces**.  

- **Ace**: A serve that directly scores a point. This occurs when:  
   - The ball lands **in-bounds** untouched by the opponent.  
   - The opponent touches the ball but is unable to return it successfully, ending the point.

---

### 3. Blocking  
Blocking happens when a player prevents an opponent's attack from crossing the net, resulting in a **point for the blocker’s team**. The metric used here is **total blocks**.  

- **Successful Block**: A block that ends the point in favor of the blocking team, often by deflecting the ball directly to the floor on the opponent’s side.

---

## Results  

### Most Clutch Attackers  

The table below highlights the **top 10 attackers** based on their hitting efficiency during clutch moments:

![Most Clutch Attackers Table](images/Most%20Clutch%20Attackers%20Table.png)

**Key Findings**:  
1. **Olivia Babcock** led all players with a **0.562 hitting efficiency** in 16 attempts, committing no errors—an impressive performance for a **freshman**.  
2. **Madisen Skinner** ranked 6th in hitting efficiency but far surpassed others in total attempts. Her frequent involvement highlights her importance during clutch moments.  
3. **Tennessee** and **Wisconsin** each placed **two players** in the top 10, reflecting their strong tournament performances.  

**Additional Insight**:  
![Least Clutch Attacker Table](images/Least%20Clutch%20Attacker%20Table.png)

At the **bottom** of the list (minimum 15 attempts), **Jenna Wenaas** from the National Champion **Texas Longhorns** posted a negative hitting efficiency. Texas' ability to win the championship despite this highlights their **roster depth**.

---

### Most Clutch Blockers  

The table below showcases the **top blockers** during clutch moments:

![Most Clutch Blockers Table](images/Most%20Clutch%20Blockers%20Table.png)

**Key Findings**:  
1. **Bekka Allick** and **Asija O’Neal** dominated as middle blockers for the two National Championship teams, Nebraska and Texas, respectively.  
2. **Andi Kreiling** (UCSB) stood out with **3 blocks** in a single clutch-time match.  
3. Players like **Anna DeBeer** and **Kendall Kipp**, who are not middle blockers, achieved high block totals, showcasing impressive defensive versatility.

---

### Most Clutch Servers  

The table below highlights the **top servers** based on total aces during clutch moments:

![Most Clutch Servers Table](images/Most%20Clutch%20Servers%20Table.png)

**Key Findings**:  
1. **Grace Chillingworth** (Pepperdine) recorded **3 clutch-time aces** in just **one tournament match**, a standout performance.  
2. **Cat Flood** and **Ayden Bartlett**, serving specialists, excelled in applying pressure during critical moments.  
3. **Arkansas** placed **two players** in the top 8, demonstrating their ability to maintain strong service pressure under pressure.  

---

### Tournament Results and Rankings  

To provide additional context for this analysis, the final **Top 15 NCAA Rankings** and the tournament bracket, including a zoomed-in view of the **Final Four**, are included below:

![Top Half of Tournament Bracket](./images/Bracket%20Top%20Half.png)  
![Final Four Bracket](./images/Bracket%20Final%204.png)  
![Bottom Half of Tournament Bracket](./images/Bracket%20Bottom%20Half.png)  

---

![Final Top 15 Rankings](./images/Final%20Top%2015.png)  

---

As shown, **Texas** was the eventual National Champion, with **Nebraska** finishing as the runner-up. These two teams consistently featured players in the **Clutch Player Analysis**, particularly in the categories of **attacking** and **blocking**.  

#### Insights:  
- **Texas and Nebraska** players appeared frequently in the clutch-time analysis. This is notable, as both teams performed exceptionally well throughout the tournament.  
- Metrics such as **hitting efficiency** remain valuable across different contexts, as they provide a standardized way to evaluate performance under pressure, regardless of the number of opportunities.  
- These findings suggest that identifying clutch-time performers is an important consideration for recruiting and team-building. While raw athletic ability is critical, so is the ability to perform consistently in high-pressure situations against strong opponents.

#### Potential Applications for Coaches:  
This analysis could be a useful tool for university athletic departments and coaching staff to identify and recruit players who excel under pressure. Teams like **Texas** and **Nebraska** demonstrate that clutch-time performance correlates with tournament success. Coaches can leverage these insights to build squads capable of thriving in high-stakes matches, ultimately improving their chances of advancing deep into the tournament.

---

## Replicating This Analysis  

To replicate this project, follow these steps:  

1. **Acquire `.dvw` Files**:  
   - Obtain play-by-play volleyball data in **DataVolley (.dvw)** format.  
   - These files are accessible through platforms like **Volleymetrics**.  

2. **Set Up the Environment**:  
   - Install **R** and **RStudio**.  
   - Install required libraries:  
     ```r
     install.packages(c("tidyverse", "datavolley", "kableExtra"))
     ```

3. **Folder Structure**:  
   Organize your files as follows:  
   ```plaintext
   project-folder/  
   ├── data/  
   │   ├── match1.dvw  
   │   ├── match2.dvw  
   ├── NCAA_2023_WVB_Analysis.Rmd  
   └── README.md  
   
## Author  

**Joshua Bastin**  
Master of Science in Business Analytics  
UCLA Anderson School of Management  

