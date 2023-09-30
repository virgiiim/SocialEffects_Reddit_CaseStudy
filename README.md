# SocialEffects_Reddit_CaseStudy

# Data
Data are collected from various subreddits pertaining to mental health and depression from 01/05/2018 to 01/05/2020.

- The folder `Emotional_Profiles` contains data about textual features extracted from user texts on a monthly basis, e.g., the file `2018-05.txt` contains the emotional profiles (in terms of textual features) of users active during May 2018.
- The folder `Emotional_Clusters` contains the cluster's centroids values across textual features. 
- The folder `Node_Labels` contains data about the node clusters identified on a monthly basis, e.g., the file `2018-05_labels.txt` contains the list of all the users active during May 2018 together with their cluster ids.

   Each file has a column `node` and a column `cluster`. A user is associated to one of the four cluster ids identified in our analysis. The cluster ids `1,2,3,4` in each file correspond to the clusters referred to as `C1,C2,C3,C4` in the article. Users are anonymized such that `1000,2` in `2018-05_labels.txt` indicates that the user id `1000` belongs to the cluster id `C2` during May 2018.

* The folder `Graphs` contains data about the discussions between users represented as pairwise interaction graphs on a monthly basis, e.g., the file `2018-05_edges.txt` contains the pairwise snapshot graph for May 2018.

  Each file has a column `Source`, `Target` and `Weight`, where the first two columns indicate the link between two users and the third one is the number of time the users discussed. Users are anonymized such that `1000,1001,3` in `2018-05_edges.txt` indicates that the two users discussed 3 times during May 2018.

* The folder `Hypergraphs` contains data about the threads of discussions between groups of users represented as hypergraphs on a monthly basis, e.g., the file `2018-05_hyperedges.txt` contains the snapshot hypergraph for May 2018.

  Each file has one column containing the list of users participating in a thread of discussion/hyperedge. Users are anonymized such that `100,1000,1001` indicates that three users participate in a hyperedge.
