# Diffusion of AI on a Trading Floor

#### The integration of technology known as "AI" has the potential to change numerous industries. However, there is a significant difference between what companies claim they can accomplish using AI and what they actually do with it. Several factors could account for such a disparity: the adoption of AI tools is costly because it tends to jeopardise an incumbent's operations; there is a scarcity of human capital trained in the field of AI; and developing AI applications may require businesses to deal with ethical and regulatory issues. Another barrier to AI adoption in knowledge-intensive businesses is "professionals." While some people may be excited to incorporate AI into their everyday job, others may feel intimidated. This project is concerned with the distribution of securities traders' perspectives on the influence AI may have on "trading floors."

#### The Aim of the project is to provide the client with a soloution to sustain diffusion of ai on the trading floor by deploying network analytics on the floor.

## Data Description
#### You distributed a survey on a major trading floor at Canary Wharf in order to get a better grasp of traders' sentiments regarding AI. The resultant dataset "tradingfloor.xml",comprises 192 replies to the following questions:

#### A trader's assessment of AI's contribution to his or her productivity and effectiveness in stock analysis (1 = not at all; 10 = significantly). This variable is given as the node attribute ai in the datasets. You also know where the traders are on the floor thanks to the client's assistance. There are six zones, each of which houses 32 people (16 individuals on each side of the zone). The above-displayed image depicts the layout of the trading floor. The position of traders is represented in the dataset as two node properties, x-pos and y-pos.

### The python code to the solution is given in the file "Diffusion_AI.ipynb"

### Following a comprehensive study of the data and mapping the network, the following findings and suggestions were made to the customer in order to continue the spread of AI on the trading floor:

#### The Traders' opinions are mapped onto the knowledge exchange network as shown below, where the darker nodes represent the traders with a highly favorable view on AI. The lightest nodes are the ones who disagree that AI might increase productivity and effectiveness in evaluating securities. Clearly, some fewer traders have a definite positive opinion on AI being helpful, which is almost equal to the number of people having a strong negative sentiment. The knowledge network shows us that, on average, the opinion on ai in the whole network is relatively moderate or more minor. Also, the size of nodes represents the degree of distribution, which shows that most of the nodes in the network have a high degree distribution, i.e., four on average.
<p align="center">
<img width="363" alt="image" src="https://user-images.githubusercontent.com/66077662/189641192-8e50320d-4207-4955-bfb5-0db94dd74ba5.png">
</p>
<h5 align="center">Knowledge Network</h5>


#### From the closeness centrality mapped onto the network, which represents the closeness corresponding to the color Scale, we can infer that there isn't a core-periphery structure as it doesn't mean any high closeness among the nodes.
<p align="center">
<img width="467" alt="image" src="https://user-images.githubusercontent.com/66077662/189641227-3c1f47e6-3ee3-498c-aa06-82a8ec8a80a7.png">
</p>
<h5 align="center">Closeness Centrality</h5>


#### The trader's opinions are mapped on to a physical layout of the trader's locations on the trading floor, which is known to be divided into six zones, which comprise 32 traders with 16 traders on each side, the darker nodes are the traders having a strong positive opinion about AI, and the lightest nodes are ones having a strong negative sentiment, the nodes with higher degree distribution are more prominent in size when compared to the ones with less degree distribution. We can infer from the network that there are nodes with positive opinions which are located next to each other, which means that one of Neighbour's must have been influenced to some degree previously, which made them strongly believe in AI, in general, from the mapping the sets of neighboring nodes seem to have an identical level of opinion towards AI.
<p align="center">
<img width="339" alt="image" src="https://user-images.githubusercontent.com/66077662/189641263-5f9f6c59-9e8a-4c31-8340-03c2eb16c4ec.png">
</p>
<h5 align="center">Knowledge Network on Trading Floor</h5>

#### There were six communities detected using the best partition community detection algorithm shown below, which doesn’t infer anything about the opinion among the traders, except that some communities have a favorable opinion on average.
<p align="center">
<img width="315" alt="image" src="https://user-images.githubusercontent.com/66077662/189641450-d050e260-78e8-4479-818c-62a4b7dcec7e.png">
</p>
<h5 align="center">Communites Detection</h5>

#### From the analysis, we can observe that the network doesn’t exhibit any core periphery. The communities detected also doesn’t say much about t opinions among traders, betweenness centrality of the network was also checked from which we can interpret that there is a significant difference in the betweenness of the node of which there are nodes with very high betweenness, which can be seen from the network below corresponding to the color scale.
<p align="center">
<img width="451" alt="image" src="https://user-images.githubusercontent.com/66077662/189641670-00761238-58e7-4715-9b70-49f2293ae51f.png">
</p>
<h5 align="center">Betweeness Centrality</h5>

<p align="center">
<img width="458" alt="image" src="https://user-images.githubusercontent.com/66077662/189641691-15ca3f1c-8b74-4bb5-a039-7a2934b6f253.png">
</p>
<h5 align="center">Eigenvector Centrality</h5>

<p align="center">
<img width="320" alt="image" src="https://user-images.githubusercontent.com/66077662/189641709-b5236187-2028-4503-bea2-feb41ab43a9e.png">
</p>
<h5 align="center"> Before Cascading (Early Adopters)</h5>


<p align="center">
<img width="318" alt="image" src="https://user-images.githubusercontent.com/66077662/189641733-6508782b-7fee-4971-bdc2-64dd9524646c.png">
</p>
<h5 align="center">After Cascading</h5>


#### From the networks shown above, diffusion and cascading are performed considering the nodes having a strong positive opinion (10) as the early adopters. The number of early adopters here is ten. After cascading, the number of adopters increased to 27, which means the opinion of the early adopters influenced 17 other nodes. If the nodes with opinions greater than or equal to 8 were taken as early adopters who are 25 in number, it would result in an adoption of 72 nodes. Hence the diffusion is less because there are only ten early adopters with a solid positive opinion.

#### The main network-related obstacles observed are: 
#### 1. The nodes with the highest betweenness centrality’s carry a negative or neutral opinion towards AI, and the nodes with a definite positive view, on the other hand, have lesser betweenness centrality values. 

#### 2. significantly fewer early adopters with a strong positive opinion towards AI. 

#### 3. The nodes with high eigenvector centrality, i.e. strong influence in the network, have a strong or mild negative opinion towards AI.

#### Looking at the network-related issues inferred from the knowledge network, I would recommend that the nodes with higher betweenness be influenced by conducting informative sessions about the advantages of AI to increase the spread of positive opinions in the network. The traders who don’t tend to high risks can be filtered and trained with the AI tools to decrease the risk on the client and might be helpful in the diffusion of positive opinion in the network. The number of early adopters can be increased by training the traders on the trading floor to work with AI. Also, the client can conduct AI-based simulation trading events to raise awareness about AI tools and their effectiveness in evaluating securities. 
#### The present traders who have a strong positive opinion about AI tools can be trained to network with other traders, including those in the different zones and create a denser knowledge exchange network by sharing knowledge with a significant number of traders. This would help spread positive opinions in the network.




 
