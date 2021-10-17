# Location-based-Privacy-Protection
Protection of personal data is vital to individuals. With the prevalence of cyber-crime, it is important to leverage the power of artificial intelligence to protect the user. The more someone else knows about a person and their whereabouts, the more power they can have over that person. This power takes the form of influence over their decisions, perhaps reveals to others their behaviours, where they live, and subsequently can affect their reputation or even safety. 
This review will provide an exploration into three methods of obsuring a person’s geographical location when using location-based services. It will explain to the user how artificial intelligence can be used in their favour.

Unfortunately, there is no perfect protection of privacy because location-based services (LBS) rely on the device’s accurate location to provide services, such as restaurant recommendations or games like Pokemon. There must be a balance between total privacy and the exposure of information on an individual. 
Three obfuscation-based mechanisms were compared on their data privacy efficacy, data utility, and ease of implementation. These mechanisms are: location generalisation (cloaking), location perturbation (differential privacy), and location spoofing (using dummy locations). 
Gowalla is a location-based social networking website where users share their locations by checking-in.  
A subset of the Gowalla dataset was used to evaluate these three mechanisms. 

Without any obfuscation (as a baseline), 74-77% of users locations can be easily discovered in the dataset. This a level of only 23-26% privacy. At the same time, this allows 100% utility and no overhead in data processing. 

Application of the three algorithms to the Gowalla data subset resulted in the following rates of success: 
Differential privacy using logistic regression with an epsilon of 0.8 afforded the users the best level of privacy at 98%. Assuming the Laplacian noise can be removed at the receiving end, it provides 100% utility and low overhead. 
The two k-anonymity algorithms, l-diversity and t-closeness were next in terms of privacy protection. Both algorithms delivered 72% privacy but, the utility was diminished for the t-closeness algorithm as the aggregations were too large to give accurate recommendations to users. 
The last methodology of location spoofing fared the worst of the three methods. This was not due to the level of privacy afforded (75%), but the overhead for this methodology is very high, with each server having to create and process a multitude of dummy locations. The utility could be 100% if the dummy locations could be efficiently removed at the receiving server. In addition, any improvements on privacy protection would require additional geographical semantics to provide further cloaking of the user’s location against location-based attacks.
