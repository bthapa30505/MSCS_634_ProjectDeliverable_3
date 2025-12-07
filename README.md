# MSCS_634_ProjectDeliverable_3

## Summarize key insights from your classification, clustering, and pattern mining efforts.

Classification Insights: Predictive Intervention
The analysis revealed that the Tuned Naïve Bayes model achieved the highest performance among classification models, with an accuracy of 0.9281 and an F1 score of 0.9536. This makes it a robust tool for predicting whether a student is likely to achieve a high or low exam score. By applying this model to historical or current student data, such as previous scores, attendance, and demographics, educational institutions can identify students at high risk of low performance long before exams occur. This predictive capability enables targeted interventions, allowing schools to prioritize resources such as remedial classes, counseling, tutoring, or parent engagement. By shifting from reactive to proactive support, institutions can maximize the effectiveness of their academic assistance programs.

Clustering Insights: Differentiated Support Groups
K-Means clustering revealed two distinct student groups primarily differentiated by previous scores and family income, indicating a strong link between socioeconomic factors and academic performance.

Cluster 0 (Lower Previous Scores, Low Family Income): This group contains the lowest percentage of high performers (20%). Interventions for these students could focus on addressing foundational skill gaps and providing additional material or financial resources.

Cluster 1 (Higher Previous Scores, Medium Family Income): While performing better overall, 70.7% of students in this cluster still score low. Interventions here may target advanced subject enrichment, motivation, or strategies to maintain academic momentum.

These clusters provide a clear, data-driven basis for resource allocation, enabling the school to distribute scholarships, tutoring slots, or counseling time where it is needed most, ensuring equitable support.

Association Rule Insights: Causal Factors and Policy
Association rule mining highlighted strong conditional relationships between various factors and student performance outcomes.

Risk Mitigation: High-confidence rules, such as Attendance_Low ⇒ Exam_Score_Low (98.16% confidence, 1.17 lift), indicate nearly certain predictors of poor performance. This underscores the importance of attendance as a non-negotiable factor in academic success. Schools should implement or strengthen policies to monitor attendance closely, such as mandatory check-ins or automated alerts for parents and counselors.

Resource Management: Rules like Access_to_Resources_Low ⇒ Exam_Score_Low (91.16% confidence) and Access_to_Resources_Medium ⇒ Exam_Score_Low (85.18% confidence) reveal that inadequate access to resources is a major barrier. The institution should audit and enhance resource accessibility, including library hours, computer labs, and textbook loan programs, particularly for students with reported low access. Interestingly, the rule Access_to_Resources_Low ⇒ Internet_Access_Yes (93.22% confidence) suggests that “low resources” may not mean a lack of internet but a deficiency in other critical tools, allowing the school to refine its understanding of resource gaps.

## Discuss the practical relevance of your findings and their real-world applications.

The study shows that data models can help schools improve student success. The Tuned Naïve Bayes model can predict which students may perform poorly, so schools can provide help early, like mentors, tutoring, or extra classes. Clustering and association rules show which students need more support based on past scores and family income. Schools can use this to give resources fairly, such as free tutoring or technology for those who need it most. Attendance is very important, and low attendance strongly predicts low exam scores, so strict monitoring and quick intervention can help. The findings also suggest that resources and student effort matter more than teacher quality alone. Overall, these tools help schools make smart, practical decisions to support students and improve learning outcomes.

## Identify challenges encountered and describe how they were addressed.

During this project, I faced several challenges, each requiring a tailored solution. One major challenge was selecting the most suitable models for the dataset I had chosen in Project Deliverable 1. For the classification task, the best model was identified based on accuracy and F1 score. I tested three different models and selected the one that performed the best. In contrast, for clustering, it was less clear which model would yield the most meaningful results for my dataset. To address this, I applied a similar strategy, experimenting with two different clustering models to explore the diverse insights each could provide. Another issue I faced was while using Jupyter Notebook was that the kernel kept crashing when processing heavy copmutation. I resolved this by restarting the kernel and ensuring that data was loaded in smaller, manageable chunks to prevent memory overload.
