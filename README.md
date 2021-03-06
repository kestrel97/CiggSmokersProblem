# CiggSmokersProblem

Contirbutors:

Faraz Murtaza	k16-4054
Okesh Kumar	k16-4026
Syed Hamza	k16-4059

The cigarette smokers’ problem is a concurrency problem in computer science, originally described in 1971 by Suhas Patil.
In this problem The Agent represents the Operating System and the smokers represent the processes. In this problem The Agent (Operating System) should allocate resources to smokers (Processes) and at the same time avoid Deadlock.

Problem Description:
Assume a cigarette requires three ingredients to make and smoke: tobacco, paper, and matches. There are three smokers around a table, each of whom has an infinite supply of one of the three ingredients — one smoker has an infinite supply of tobacco, another has paper, and the third has matches.
There is also a non-smoking agent who enables the smokers to make their cigarettes by arbitrarily selecting two of the supplies to place on the table. The smoker who has the third supply should remove the two items from the table, using them (along with their own supply) to make a cigarette, which they smoke for a while. Once the smoker has finished his cigarette, the agent places two new random items on the table. This process continues forever.

Three semaphores are used to represent the items on the table; the agent increases the appropriate semaphore to signal that an item has been placed on the table, and smokers decrement the semaphore when removing items. Also, each smoker has an associated semaphore that they use to signal to the agent that they are done smoking; the agent has a process that waits on each smoker's semaphore to let it know that it can place the new items on the table.



