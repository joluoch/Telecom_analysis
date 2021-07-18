# Telecom_analysis
This notebook is from a training from @10academy. I conducted customer segmentation on a telcom industry dataset. 
clusterting customer based on Engagement and experience 

For the engagement cluster the following metrics were used 
●	sessions frequency 
●	the duration of the session 
●	the sessions total traffic (download and upload (bytes))

For  the experence metrics the following metrics were used 

●	Average TCP retransmission
●	Average RTT
●	Handset type
●	Average throughput

We then calculated the satisfaction score of each customer by first , using the Euclidean Distance between the  user data point & the less engaged cluster for the engagement cluster and the user data point & the worst experience’s cluster for the experience cluster 
 From that , the average of both engagement & experience scores as  the satisfaction score
 
 we then predict the score using a logical regressor and save the model into a pickle 
 we also cluster the satisfaction score using kmean and saves the model
 
 finaly we develop a dashboard the accepts the engagement score and experence score the it is run in the kman model and the customer is graphed in their cluster 
