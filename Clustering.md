An unsup ml where the goal is to group sample that have fea close related to eachother into on group by calc the dist of each sample

- No label given, model must group it themself (unsup learning)
- Model will gave two type of cluster
	- Hard Group: every data point belongs to **exactly one** cluster. It is a binary decision: you are either in the group or you are out.
	- Fuzzy Group: data points can belong to **multiple clusters** at the same time. Instead of a "Yes/No" assignment, each point has a **probability or membership score** for every cluster.