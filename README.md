## Title:
Testing BFS sampling approach as a generation method of representative samples

## Abstract: 
The authors of the paper claim that the BFS sampling approach could not generate representative samples. Our aim is to verify this thesis. Hence, we are going construct a new dataset, then validate its representativeness using Kolmogorov-Smirnov test as the authors in the paper, and finally repeat some investigations made by the Hai L. et al. In order to generate the dataset we will randomly generate some Twitter IDs and check if there exists a corresponding Twitter user. Then we will use those egos as sources to launch BFSs. The nodes of a search graph are Twitter users while edges are both follower and followee relationships. We will generate a dataset which size will be approximately equal to the one used by the authors of the paper. Finally, using new dataset we will repeat verifications of some prepositions. 

## Research questions
1. Is the BFS sampling approach representative based on Kolmogorov-Smirnov test?
2. How many sources we need to to generate a representative dataset?
3. Are the authors' prepositions agree with the conclusions drew from our dataset?

## Proposed datasets
- Dataset generated in a way described below

## Methods
**Dataset generation** We will try different number of sources (100-1000) for BFS and choose the best dataset using Kolmogorov-Smirnov test. To download the data we will use Twitter API
**Verification of prepositions** We have decided to focus on one preposition from each section, i.e. "Circadian rhythms" (usage), "Dunbar’s number" (structure), and "Influential hypothesis" (information diffusion).

## Proposed timeline
- **Week 1:** Dataset generation
- **Week 2:** Verification of chosen prepositions
- **Week 3:** Prepare report and a short video

## Organisation within the team:
- Viktor will find out how to get an access to Twitter API
- Maciek will write BFS and the setup for fetching data using Twitter API
- Maciek will clean the data and verify two prepositions (usage and structure)
- Viktor will verify the third preposition (information diffusion)
- Maciek will organise and clean the code, and work on making a data story notebook
- Viktor will prepare video