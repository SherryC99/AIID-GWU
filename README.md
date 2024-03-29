[Tentative Work Schedule](https://docs.google.com/spreadsheets/d/1wKuUxDjGla84A0PknrEduSr4THQX8Uk1tx9OrzWIkRs/edit?usp=sharing)

[Tentative Work Flow Map](https://github.com/SherryC99/AIID-GWU/blob/d1cc0b1280c780315bd3dda38665957115c34d5e/Appendices/AIID%20Project%20by%20Group%202.pdf)

[Project Proposal](https://github.com/SherryC99/AIID-GWU/blob/d1cc0b1280c780315bd3dda38665957115c34d5e/Appendices/UL-DSRI.docx.pdf)

## 1. Executive Summary

The project aims to computationally analyze the changing trends and rhetoric in AI journalism using data from the AI Incident Database (AIID). By leveraging natural language processing (NLP) techniques such as topic modeling, sentiment analysis, and named entity recognition, the goal is to uncover insights into how the media reports incidents and harms related to AI over time. By examining over 600 incident reports indexed by AIID, the project seeks to understand shifts in sentiment, language usage, and thematic trends in media coverage surrounding AI systems The findings will not only benefit the AIID but also inform stakeholders in AI safety, governance, and compliance.

## 2. Problem Understanding

The AI Incident Database (AIID) records real-world harms caused by AI systems and aims to raise awareness among stakeholders. However, since its inception in 2019, the landscape of AI journalism has evolved, impacting how incidents are reported and perceived. The project seeks to address the following questions: Have certain AI trends fallen away over time? Has sentiment regarding AI harms changed in particular publications? Where do media reports agree or differ in sentiment and language when describing AI harms?

The AI Incident Database (AIID) indexes incidents and harms caused by AI systems based on journalistic reports, but the nature of AI journalism has evolved over time. This project seeks to understand how trends in AI reporting have shifted, whether certain AI topics have garnered more attention than others, and how the sentiment surrounding AI harms has changed in different publications. By answering these questions, the project aims to enhance the understanding of AI discourse and improve the indexing of incident reports in the AIID.
Introduction to the challenges and importance of analyzing media coverage of AI,Explanation of the need for sentiment analysis in understanding public perception and Overview of the specific research questions addressed in the project are the main problem understandings dealt here.


### Literature review on Media Biases

[Literature review 1 Source](https://www.tandfonline.com/doi/full/10.1080/21670811.2021.1969974)

**Summary**: 

The article examines how AI-generated news can mitigate perceptions of hostile media bias (HMB) through the activation of the machine heuristic, which suggests machines are more objective and unbiased than humans. Using an online experiment, it finds that stories presented as sourced from AI journalists lower HMB, particularly among individuals with more extreme partisan attitudes. The effect of machine cues on reducing perceived bias suggests potential for AI in journalism to address challenges of public distrust and political polarization.

[Literature review 2 Source](https://www.tandfonline.com/doi/full/10.1080/14680777.2023.2263659)

**Summary**: 

The study, "The Invisible Women: Uncovering Gender Bias in AI-generated Images of Professionals," explores gender bias in AI-generated images across four professions (law, medicine, engineering, and scientific research). Analyzing 99 images from nine text-to-image generators, the study finds a significant gender bias, with men represented in 76% of images and women only in 8%. This bias is consistent across all professions and varies among different AI generators, highlighting the need for more inclusive AI design to address gender inequalities.


[Literature review 3 Source](https://www.psu.edu/news/information-sciences-and-technology/story/trained-ai-models-exhibit-learned-disability-bias-ist/)

**Summary**:

The study conducted by researchers from Penn State's College of Information Sciences and Technology investigates biases against people with disabilities in natural language processing (NLP) algorithms and sentiment analysis models. Published in 2023, the paper titled "Automated Ableism" addresses the increasing use of AI-driven sentiment analysis tools and highlights concerns regarding the biases embedded in these systems. By analyzing social media conversations related to disabilities, the researchers demonstrate the presence of significant bias in sentiment and toxicity analysis models, with statements about disabilities often receiving more negative and toxic scores. The study emphasizes the need to address disability bias in AI models to mitigate social harm and promote inclusivity in AI development and deployment.

[Literature review 4 Source](https://www.mdpi.com/2073-431X/12/2/37)

**Summary**:

Artificial Intelligence and Sentiment Analysis: A Review in Competitive Research(2023) by Taherdoost et. al  present a comprehensive review of AI-based sentiment analysis in competitive research. They emphasize the growing importance of understanding customer sentiments for strategic decision-making. The review outlines the evolution of sentiment analysis methodologies, challenges faced, and future prospects in leveraging AI for competitive advantage.This paper reviews the application of artificial intelligence (AI) in sentiment analysis for competitive research. It explores how AI-powered sentiment analysis aids in understanding customer perceptions and competitive dynamics. The review covers literature from 2012 to 2022, highlighting the development, challenges, and prospects of AI-based sentiment analysis in competitive research.

[Literature review 5 Source](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8402961/)

**Summary**:  

Nandwani et. al(2021) delve into the realm of sentiment analysis and emotion detection from textual data, elucidating their pivotal roles in deciphering human behavior within diverse contexts. They underscore the burgeoning significance of social media platforms as repositories of human emotions and opinions, necessitating efficient computational methods for sentiment and emotion analysis. The authors provide insights into various methodologies employed, ranging from lexicon-based approaches to machine learning and deep learning techniques, while also highlighting the challenges inherent in dealing with contextual nuances and linguistic ambiguities. Moreover, they elucidate the intricate facets of emotion models, emphasizing the multidimensional nature of human emotions and the complexities involved in their automated recognition. Nandwani and Verma (2021) further expound on the critical steps involved in sentiment and emotion analysis, including dataset collection, preprocessing, feature extraction, model development, and evaluation. They stress the paramount importance of robust datasets in training accurate models and discuss the trade-offs between different analysis approaches, such as lexicon-based methods, machine learning algorithms, and deep learning architectures. Additionally, the review underscores the pivotal role of pre-processing and feature extraction techniques in enhancing the performance of sentiment and emotion analysis systems. By offering a comprehensive synthesis of existing methodologies, challenges, and future directions, the paper serves as a valuable resource for researchers and practitioners aiming to navigate the intricate landscape of sentiment analysis and emotion detection from textual data.

[Literature review 6 Source](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8967082/)

**Summary**:  
The study by Peters (2022) delves into the underexplored realm of algorithmic bias in artificial intelligence (AI) systems concerning individuals' political orientation. While existing research predominantly scrutinizes biases related to gender and racial identity, Peters argues that biases based on political orientation, being less constrained by societal norms, pose distinctive challenges. The paper emphasizes the increasing role of AI systems in pivotal decision-making processes, such as job recruitment or loan eligibility, and contends that biases rooted in political orientation may be harder to detect and eradicate than their gender or racial counterparts. By shedding light on the unique risks associated with algorithmic political bias, the paper calls for heightened awareness and examination within the AI community. His paper fills a crucial gap by introducing the concept of algorithmic political bias and highlighting its distinctive challenges. The author contends that, unlike gender and racial biases, there are fewer potent societal norms to restrain political biases, making them more pervasive and influential in AI algorithms. The study underlines the potential harm caused by algorithmic political biases, particularly as algorithms can now involuntarily uncover individuals' political orientations. The analysis suggests that changes in social norms regarding responses to political differences might mitigate such biases but cautions that these norms have complexities, complicating the task of addressing algorithmic political bias effectively.

## 3. Methodology: Data Analyzed

[Python Code](https://colab.research.google.com/drive/1YuGVrqoseHxnzrCrrR0MG_plzyaT_yBg?usp=sharing)

* The project will utilize media reports indexed in the AI Incident Database (AIID) to analyze trends and characteristics in AI journalism. The dataset consists of over 600 unique incident reports sourced from 3,500+ journalistic articles. These reports cover a wide range of AI-related topics and incidents, providing rich data for analysis. Additionally, the project may consider expanding the analysis to include other media-type datasets if necessary. Analyzing a corpus of AI-related journalistic reports sourced from the AIID, exploring trends, sentiment, and language shifts over time in reporting on AI incidents, identifying common themes, entities, and relationships within the dataset are the main analyzations.

## 4. Methodology: Analytics Techniques
* Python: NLP packages
* MongoDB Compass
* Google Colab
The analysis will primarily employ natural language processing (NLP) techniques such as topic modeling, sentiment analysis, and named entity recognition. These techniques will help uncover patterns, trends, and sentiment changes in AI journalism over time. Employing data visualization methods for communicating insights effectively. We leverage a range of inbuilt concepts like mathematical and statistical methodologies, including linear algebra concepts such as Singular Value decomposition and statistical methods. 



## 5. Results/Conclusions/Recommendations
Upon completion of the analysis, the project will present insights into the changing trends and rhetoric in AI journalism. The findings will highlight shifts in media attention towards different AI topics, changes in sentiment surrounding AI harms, and variations in reporting styles across different publications. For example, there may be fluctuations in the frequency of certain terms or the prevalence of positive/negative sentiment in reporting on AI incidents. These insights will not only benefit the AI Incident Database (AIID) but also provide valuable information for stakeholders in AI safety, governance, and compliance. Understanding these sentiment patterns provides valuable insights into public perception and media discourse surrounding AI. Our analysis underscores the dynamic nature of AI journalism, influenced by various factors such as technological advancements, public discourse, and media narratives.

Recognizing these dynamics is essential for accurately capturing and indexing AI-related incidents in databases like AIID. Contextual understanding is crucial when interpreting media coverage of AI incidents. While sentiment analysis provides valuable insights, considering the broader context in which these sentiments are expressed is essential. This includes factors such as the tone of the article, the credibility of the source, and the specific circumstances surrounding the incident.Continuous monitoring and adaptation are recommended due to the dynamic nature of AI journalism. This involves regularly updating sentiment analysis models, refining topic modeling techniques, and staying informed about emerging trends in media coverage. Collaboration with industry experts ensures that our analysis accurately reflects the complexities of AI-related incidents portrayed in the media. To capture nuanced shifts in reporting, further investment in advanced NLP techniques is advised. These techniques offer the potential to provide more detailed insights into sentiment, language usage, and thematic trends in AI journalism.


## 6. Potential Next Steps section 
Potential next steps include refining the analysis to uncover deeper insights, exploring additional NLP techniques. Explore ensemble modeling approaches to enhance sentiment analysis accuracy.Recommendations may also be made for improving the indexing of incident reports in the AIID and tracking discourse about AI and related harm more effectively. Expand the scope of data collection to include a broader range of sources, languages, and regions. This will provide a more comprehensive understanding of global perspectives on AI-related incidents and trends.Explore techniques for detecting and mitigating biases in media coverage of AI incidents. This could involve developing algorithms to identify biased language, assessing the impact of bias on public perception, and implementing strategies to promote balanced reporting.Analyzing cross-domain influences on media coverage can provide a more holistic understanding of the socio-cultural factors shaping perceptions of AI.


## 7. Risk Considerations section
One potential risk is that the dataset may not contain sufficient information to adequately answer the research questions. In such cases, adjustments to the scope of the analysis or exploration of additional data sources may be necessary. Risk of bias in media reporting may influence the accuracy of sentiment analysis and trend identification.Ethical considerations arise regarding data privacy and consent in analyzing journalistic content. Additionally, potential challenges exist in interpreting and contextualizing findings within the broader landscape of AI research and development. Other risk considerations include the potential for algorithmic biases in the NLP model used for sentiment analysis, the risk of misinterpretation of results due to complex linguistic nuances, and the possibility of unintended consequences stemming from recommendations based on the analysis. Furthermore, there may be risks associated with relying solely on media reports for data analysis, such as incomplete or inaccurate information leading to flawed conclusions. 


## 8. Appendices
Links to the data used, code developed for the analysis, and any additional resources relevant to the project will be included in the appendices for reference. This ensures transparency and reproducibility of the analysis and allows for further exploration. Links to relevant literature and resources consulted during the project will also be included. Moreover, appendices might contain data dictionaries or schemas explaining the structure and meaning of the datasets used, along with any additional supplementary materials such as presentation slides, repository files etc. created for dissemination purposes.

[Tentative Work Schedule](https://docs.google.com/spreadsheets/d/1wKuUxDjGla84A0PknrEduSr4THQX8Uk1tx9OrzWIkRs/edit?usp=sharing)

[Tentative Work Flow Map](https://github.com/SherryC99/AIID-GWU/blob/d1cc0b1280c780315bd3dda38665957115c34d5e/Appendices/AIID%20Project%20by%20Group%202.pdf)

[Project Proposal](https://github.com/SherryC99/AIID-GWU/blob/d1cc0b1280c780315bd3dda38665957115c34d5e/Appendices/UL-DSRI.docx.pdf)

