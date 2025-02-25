## Customer-Clustering
# 1. Background information
-This project is based on a simulated customer data set of Stratton AE Banking (Yildirim and Kubler, 2023). As described, Stratton AE Banking is a joint venture operating in e-banking service, and it is so far, successfully attracted young investors and customers. As a long-term ambition, they wish to appoach the strong existing customer base of their venturers - a private banking house. However, there are some risks associated with simply proaching all customers as the new technology of data driven and digital experience might disturb some current intimate relations, which is crutial to the success of the venturer bank.
-Therefore, the managment requests to conduct a customer segmentation analysis to identify the suitable customer segments which are open to try new experience with the e-banking services of Stratton AE Banking.

# 2. EDA
First of all, we should obtain the knowledge about the available data set to gain basic understanding about the problem at hand. In total, we have a data set size of 10,750 x 29, which means the customer data base contains 10,750 identifiable customers with 29 types of information stored (from now onward, we call them variables). These variables indicate their personal information such as Age, Income, Household Size. etc and alsao the information related to the city where they live, for example Mean Income of the City or Mean House Prize of the City.

The data set also provided us the explanation of each variable to ensure the correct interpretation and prevent distortion might resulted from misunderstanding.

Once again, with more than 10k customers, approaching all of them in terms of offering new services might risk the consistent experience of long-term customers while not secure a profitable outcome. Therefore, implying some clustering methods based on provided information relating to customers and their living background might help to allocate them to targeted and non-targeted segments for an efficient approaching in terms of new services.

# 3. Customer Segmentation/Clustering
The main idea of clustering is to identify a several groups that objects within a group are more similar to each other than objects in other groups. In this case, when all the provided variables are numeric, we imply Euclidean distance to perform clustering.

Before running any clustering analysis, we must consider the scale of variable. It is obvious that the values of Income variable are always much greater than that of Age or Household Size. This variability has great effects when calculating Euclidean distance as the variables with much higher value easily dominate the other variables. Therefore, it is neccessary to standardise all variable, bring them to a same scale where the mean value is 0 and standard variation is 1. The standardise step, hence, ensures all variables are equally considered in clustering.


