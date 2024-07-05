# The Role of Gender: Gender Fairness in the Detection of Depression Symptoms on Social Media

### Abstract
AI systems for depression detection on social media have been continuously improving their performance, showing that meaningful patterns can be found in the data. While many machine learning models used to detect depression are opaque, models predicting depression symptoms can often provide more explainability [1]. Research has shown that some depression detection datasets with data collected from social media exhibit gender biases [2] [3], but no research has investigated gender bias for a symptom dataset yet. Therefore, this thesis aims to answer the following research problems: To what extent is gender bias present in the BDI-Sen dataset [4] and how does a classifier trained on it perform for different genders? How can any present gender bias be mitigated? A statistical analysis reveals that the dataset shows some gender bias that reflects gender differences in depression symptoms. Analysis of mentalBERT classifiers trained on the dataset identifies several biases across the different symptoms, particularly in terms of predictive equality, with the majority of the bias favoring males. Applying synonym replacement, back-translation and oversampling as data augmentation strategies helps reduce the bias, but does not remove it completely.

For further results, the thesis can be consulted.


### Usage
Per section
All code was written with Jupyter Notebook. It has been altered such that authentication and identifiable information cannot be found, and usage requires Reddit API authentication for the creation of the GABDI-Sen dataset, and an authentication token for the mentalBERT model implementation from Huggingface. Furthermore, datasets and models are not included in the repository and access to them needs to be requested from the respective authors. The code for the dataset explorations, as well as the fairness analysis of the GABDI-CV model and the creation of the GABDI-Sen dataset have been sorted in folders for ease of view. Apart from these scripts, this repository contains the code for data augmentation, fairness measures on the replicated and the category model, and the mentalBERT implementation. Necessary requirements and libraries as used for this code are listed in the Requirements file.

### Acknowledgements
Thank you to my supervisors, Heysem Kaya and Gizem Soğancıoğlu, for the helpful insights and feedback throughout this project. Your weekly comments helped shape and improve this research, and the tea was always very appreciated! Also many thanks to Dong Nguyen for taking the time to read this work and for providing many helpful comments to the proposal.

### References

1.  Zhang, Z., S. Chen, M. Wu and K. Zhu, “Symptom identification for interpretable detection of multiple mental disorders on social media”, Proceedings of the 2022 conference on empirical methods in natural language processing, pp. 9970–9985, 2022

2. Aguirre, C., K. Harrigian and M. Dredze, “Gender and racial fairness in depression research using social media”, arXiv preprint arXiv:2103.10550 , 2021

3. Cheong, J., S. Kuzucu, S. Kalkan and H. Gunes, “Towards Gender Fairness for Mental Health Prediction”, International Joint Conferences on Artificial Intelligence Organization, 2023, https://www.repository.cam.ac.uk/handle/1810/349873.

4.  Perez, A., J. Parapar,  ́A. Barreiro and S. Lopez-Larrosa, “BDI-Sen: A Sentence Dataset for Clinical Symptoms of Depression”, Proceedings of the 46th International ACM SIGIR Conference on Research and Development in Information Retrieval , pp. 2996–3006, 2023


Other research used in this project:

Losada, D. and F. Crestani, “A Test Collection for Research on Depression and Language Use”, Proc. of Experimental IR Meets Multilinguality, Multimodality, and Interaction, 7th International Conference of the CLEF Association, CLEF 2016, pp. 28–39, Evora, Portugal, September 2016

Ji, S., T. Zhang, L. Ansari, J. Fu, P. Tiwari and E. Cambria, “MentalBERT: Publicly Available Pretrained Language Models for Mental Healthcare”, Proceedings of LREC , 2022.

Wei, J. and K. Zou, “EDA: Easy Data Augmentation Techniques for Boosting Performance on Text Classification Tasks”, Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing and the 9th International Joint Conference on Natural Language Processing (EMNLP-IJCNLP), pp. 6383–6389, Association for Computational Linguistics, Hong Kong, China, Nov. 2019, https://www.aclweb.org/anthology/D19-16

Costa-jussa, M. R., J. Cross, O. Celebi, M. Elbayad, K. Heafield, K. Heffernan, E. Kalbassi, J. Lam, D. Licht, J. Maillard et al., “No language left behind: Scaling human-centered machine translation”, arXiv preprint arXiv:2207.04672 , 2022
