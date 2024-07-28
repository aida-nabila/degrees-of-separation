# Background 
According to the Six Degrees of Kevin Bacon game, anyone in the Hollywood film industry 
can be connected to Kevin Bacon within six steps, where each step consists of finding a film 
that two actors both starred in. 

In this problem, we’re interested in finding the shortest path between any two actors by 
choosing a sequence of movies that connects them. For example, the shortest path between 
Jennifer Lawrence and Tom Hanks is 2: Jennifer Lawrence is connected to Kevin Bacon by 
both starring in “X-Men: First Class,” and Kevin Bacon is connected to Tom Hanks by both 
starring in “Apollo 13.”

![image](https://github.com/user-attachments/assets/57a3b2bd-1840-4706-90cf-8c9a4557dc8a)

# Data
The distribution code contains two sets of CSV data files: one set in the large directory and 
one set in the small directory. Each contains files with the same names, and the same 
structure, but small is a much smaller dataset for ease of testing and experimentation. 
Each dataset consists of three CSV files. 

In people.csv you’ll see that each person has a unique id, corresponding with 
their id in IMDb’s database. They also have a name, and a birth year. 

In movies.csv you’ll see here that each movie also has a unique id, in 
addition to a title and the year in which the movie was released. 

The file stars.csv establishes a relationship between the people 
in people.csv and the movies in movies.csv. Each row is a pair of a person_id value 
and movie_id value. The first row (ignoring the header), for example, states that the person 
with id 102 starred in the movie with id 104257. Checking that 
against people.csv and movies.csv, you’ll find that this line is saying that Kevin Bacon starred 
in the movie “A Few Good Men.”
