## Development Log:

**April 9 (Week 1):** In this meeting, we decided on the Higgs Twitter Dataset as our final project dataset. We then formed our leading question and committed our project proposal and team contract to GitHub.

**April 16 (Week 2):** In this meeting, we made the basic structure for our nodes, with a user being represented as a node. We then imported all the datasets, though it took us time to figure out how to upload a file that was 172 MB large. One of the members managed to do it through Git Large File Storage (LFS). Afterwards, we imported catch and make files from a previous lab, so that we could use/edit them to test our node creation. Another member also made a program to read in the first few lines of one of our datasets, which we will use in the future to fully process our datasets.

**April 23 (Week 3):** In this meeting, we finished making the catch and make files to test our node structure. We then discussed between implementing an adjacency matrix and a graph structure for storing the interaction/weight data of each node (user).

**April 30 (Week 4):** In this meeting, we experimented with several data containers to read the files to, before deciding on using a map. The key for each element in the map would represent the "matrix index" of the element, calculated as (user 2) * 500000 + (user 1), where 500,000 is the highest user id we can read. The value for each element would be the number of interactions between users. Through this structure, we can keep track of each user interaction (who interacts with who), as well as how many directed interactions occured. With this directional data, we began implementing our DFS algorithm, which will traverse through the "matrix" we constructed, as well as the PageRank algorithm.

**May 7 (Week 5):** In this meeting, we finished implementing the DFS algorithm and wrote most of the PageRank algorithm. We also began writing the algorithm for our force-directed visualization and included a way to add nodes, as well as calculate the forces on each node in the graph.

**May 12 (End of Week 5):** In this meeting, we finished all of our algorithms and tests and confirmed everything was working, including some bug fixes for DFS and adjacency matrix. We added a weight component to the force directed algorithm since we had access to one from PageRank and the algorithm normally does not.
