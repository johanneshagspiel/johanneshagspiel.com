---
layout: writing
title: MalPaCA
description: "👨‍👩‍👦‍👦 on the influence of sequence length on clustering"
published: True
---

## The influence of sequence length on the clustering performance of MalPaCA 

MalPaCa is a novel, unsupervised clustering algorithm, which creates based on the network flow of a software a behavioral profile representing its actual capabilities. One of the key variables affecting is performance and usability is the sequence length or how many packets it analyzes in order to group a connection to a cluster. This thesis explores different sequence length amounts as well as different positions from where to extract the packets from. The findings indicate that the current default sequence length of 20 is too high, leading in many cases to no clusters being found. 8 has been determined to be the optimal length for both performance and efficiency. Additionally, it has been established that using a windowed approach whereby a connection is being sliced into multiple, smaller connections could make MalPaCa more usable in situations where connection lengths are unequally distributed. Furthermore, MalPaCas usability as a tool has been improved by automating the clustering error metric determination, thereby providing the user with a valuable, visual measure as to how well MalPaCa has fared in creating the clusters. Lastly, MalPaCas definition of behavior was compared to the "Netflow v5" behavior definition, however no substantial performance improvements could be obtained from this change.

### Supervisor & Adivsor

 - Azqa Nadeem
 - Sicco Verwer
