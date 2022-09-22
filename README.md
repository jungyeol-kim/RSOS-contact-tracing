Tracing and testing multiple generations of contacts to COVID-19 cases: cost-benefit tradeoffs
===================================

### Abstract
Traditional contact tracing tests the direct contacts of those who test positive. But, by the time an infected individual is tested, the infection starting from the person may have infected a chain of individuals. Hence, why should the testing stop at direct contacts, and not test secondary, tertiary contacts or even contacts further down? One deterrent in testing long chains of individuals right away may be that it substantially increases the testing load, or does it? We investigate the costs and benefits of such multi-hop contact tracing for different number of hops. Considering diverse contact networks, we show that the cost-benefit tradeoff can be characterized in terms of a single measurable attribute, the \textit{initial epidemic growth rate}. Once this growth rate crosses a threshold, multi-hop contact tracing substantially reduces the outbreak size compared to traditional tracing. Multi-hop even incurs a lower cost compared to the traditional tracing for a large range of values of the growth rate. The cost-benefit tradeoffs can be classified into three phases depending on the value of the growth rate. The need for choosing a larger number of hops becomes greater as the growth rate increases or the environment becomes less conducive toward containing the disease.

### Contact Networks
![Screenshot](table.png) 
*Notes:* *p* is the rewiring probability of Watts-Strogatz networks, and *r* is the mixing parameter in data-driven network. The average degree is the average number of edges per node. The distance between a pair of nodes is the length of the shortest path between them. The diameter is the maximum value of this distance over all pairs of nodes. The average path length is the average of this distance over all pairs of nodes; only the lengths of the existing paths are considered and averaged. Clustering coefficient of a node *i*, *C<sub>i*, is defined as the ratio between the actual number of links between the neighbors of *i* and the maximum possible number of links between the neighbors of *i*. This is high if there exists a large number of edges in the neighborhood of *i*. The average clustering coefficient, *&lt;C>*, is the average of *C<sub>i* over all nodes *i*. The average degree, average path length, and average clustering coefficient are rounded to three significant figures.

#### The raw data used to construct data-driven network was previously published in *A Banerjee, AG Chandrasekhar, E Duflo, MO Jackson, The diffusion of microfinance. Science 341 (2013)*. 

### Simulations
We consider various attributes that affect the efficacy of contact tracing, involving variations of false negative rates, false positive rates, test result turnaround times, starting times of contact tracing, and level of cooperation with contact tracing and testing. You can vary the setting by entering values of interest of each codes.

e.g.)
intervention.start.inf.rate<-0 # Starting point of contact tracing, percent (%); enter 0 if contact tracing is initiated when the first individual tests positive
turnaround<-1  # Turnaround times for coronavirus test results (days)
FP.rate<-0 # False Positive rate, percent (%)
FN.rate<-11 # False Negative rate, percent (%)
cooperativity<-100  # Cooperativity (%)
