
Welcome To My NBA Project

My Goal For this project is to cluster NBA players based off of their position and stats.
With these clusters I will be able to discern the differences within each position and able to see based off of the 2017-2018 year see which type of players are most successful for a team to make the NBA playoffs.

Source of my Data: www.basketball-reference.com

In order to extract my data I used Beautiful Soup.
This is a very strong tool.

The metrics I used to find my clusters are based off of players stats Per 100 Possession and Advance Stats.
I used this metrics instead of ex:Per game stats because it would not skew towards players that have a longer career.


If you are looking through the notebook. 

Start with Scraping Folder- this is where I utilized Beautiful Soup

Then Positional Clustering from PG-C - This is where I modeled and looked at different position clustering

Finally Predictions Folder - This is where I looked at teams that make playoffs and see which cluster is more prominent with playoff teams.



From my findings for each position and the difference within each cluster.

---------------

All PG have strong assist #numbers

PG0 - Defensive PG with strong rebounding skills, doesn't take much 3's 
<br/>New-Protype Defensive PG- Lonzo,Murray,Ben Simmons, Russel Westbrook

PG1 - Fill ins aren't strong in anything particular
<br/>Normal PG/ Bench - Mario Chalmers, Darren Collison,Raymond Felton, De'Aaron Fox

PG2 - Offensive PG with strong 3 points makes and attempts, highest scoreers
<br/>Offensive PG - Eric Bledsoe, Steph Curry, Tyreke Evans, Kyrie Irving, Damian Lillard

Value
<br/>PG0 > PG2 > PG1

----------------

SG1 shoots more 2P and attempt more 2PA, higher PER(Player Effiecency Rating), more TOV, more AST and AST%
<br/>Passing 2's - Nicolas Batum, Victor Oladipo, Jimmy Butler, James Harden

SG0 shoots slightly more 3PA and makes more 3P, bench players, specialize in 3's
<br/>Shooting 2's - Marco Bellinelli, Avery Bradley, Kentavious Caldwell-Pope, Josh Hart

Value
<br/> SG1>SG0

----------------

SF0 strongest 3PA and 3P average STL - typical 3and D position
<br/> 3 and D(stl)- Trevor Ariza, Bojan Bogdanovic, Jae Crowder, Wesley Matthew

SF1 - Highest USG%, well rounded, AST high PER is high shoots 2P 
<br/> Well rounded 3's-DeMarre Carroll, Evan Fournier,Caris LeVert, Khris Middleton

SF2 - BLK, STL , Strong DBPM, Most Valubale
<br/> 3 and D(stl&blk)- Kyle Anderson, Corey Brewer, Robert Covington, Jayson Tatum

Value
<br/> SF2>SF1>SF0

----------------

PF0 low usage don't do much, shoot 3's, with very low defensive Skill
<br/> Stretch 4's No D - Jared Dudley, Dragan Bender, Quincy Acy, Pattrick Patterson

PF1 makes most 3's, Average Defense Skills
<br/> Stretch 4's Some D - Nikola Mirotic, Aaron Gordon, Rudy Gay, Tobias Harris

PF2 Blking 3p shooters hybrid, High STL
<br/> Stretch 4's Better D(Stl) - Draymond Green, Serge Ibaka, Markieff Morris, Pascal Siakam

PF3 gets most rebounds, most PF, don't shoot 3's, high BLK
<br/> Tradition PF -Trevor Booker, John Collins, JaMychal Green, Noah Vonleh

PF4 Definitely the most VORP, high Per, 2P, High BLK, High AST, OPBM
<br/> FREAKS - Giannis Antetokounmpo, Anthony Davis, Kevin Durant(listed as Pf), Lebron James

Value
<br/> PF4>PF2>PF1>PF3>PF0

-----------------

C0 - STL, BLK, Defensive strong, Can't shoot 3's, Rebound
<br/> Defensive Bigs - Steven Adams, Rudy Gobert, Derrick Favors, Jarret Allen

C1 - 3P center, Low Steals
<br/> Stretch 5's - Dirk Nowitzki, Myles Turner, Al Horford, Brook Lopez

C2 - VORP, FG, AST, STL, TRB, offensively strong, well rounded
<br/> Modern Big's - Karl-Anthony Towns, Kevin Love, Andre Drummond, Nikola Jokic

Value
<br/> C2>C0>C1

------------------


For Playoffs I found that 

PF2 Blking 3p shooters hybrid, High STL
<br/> Stretch 4's Better D(Stl) - Draymond Green, Serge Ibaka, Markieff Morris, Pascal Siakam

Were the most important in making playoffs.

--------------------------------------------------------------------------------------------------

To find my clusters I used many different types of clustering models and ended up with the most common model KMeans.
I used this model because I knew how to find what the best amount of cluster was for each model. 
There is 3 ways (that I know of ) to find the best clusters.
1. looking at intertia and finding an elbow
2. looking at silhoutte score and finding the highest score
3. Gap Statistics - where you use a random generate points without any clear clusters and use that to compare with your original data

I used 1 and 2.

After finding the clusters I went to look at the differences with each cluster and see what features were more dominant while other features weren't. 


Using the clusters I combined it with the data to find which teams that made the playoffs had which type of prominent cluster.
To no surprise Stretch 4's which has become the staple for the new NBA. 
Teams are all searching for good stretch 4's with good Defense.

-----------------------------------


