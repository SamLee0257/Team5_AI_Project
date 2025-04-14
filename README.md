# Team5_AI_Project

Team 5 final project on the use of AI in Human Resource activities. 

**Authors:** [Marshall Pender](https://github.com/marshallpender), [Drew Messick](https://github.com/drewmessick), [Sam Lee](https://github.com/SamLee0257), [Thomas Lavelle](https://github.com/tlav03)

**Project Scope** 

- To design and develop an AI-based system that assists human resources (HR) departments in screening resumes efficiently. 

The system will include:

1. A resume scanning tool integrated into a web-based application for companies to use in their hiring process.
2. A deep learning model to classify whether a candidate's resume is qualified for a specific job role or not based on predefined criteria (e.g., skills, experience, education).
3. The integration of AI to streamline the candidate selection process and reduce human bias.

**Project Details** 

*Project Statement:* How can human resource departments efficiently manage and evaluate a large volume of resumes? ​

Solution: We developed a model that classifies resumes as "qualified" or "not qualified" based on key attributes. Additionally, we created a user-friendly website powered by AI to filter resumes, automatically generating a Google Sheet that lists resumes matching the specified criteria.

*Deep Learning Resume Classification Model*: For this project, we generated synthetic data to simulate grad school applications and classify candidates as qualified or not based on a predefined list of desired and undesired attributes (e.g., skills, experiences). To introduce realism, we added noise to the dataset—ensuring that "qualified" entries still contained some unqualified traits and vice versa. Using this dataset, we trained a deep learning model that was able to predict candidate qualification with nearly 90% accuracy.

*Website Creation Via Vibe Coding*:
We utlizized Claude AI using vibe coding to assist in creating the website we wanted. Our **original prompt** to Claude was as follows: 

"I am building a resume filter website using Google Apps Script. I want to be able to filter a file of resumes stored as google docs on google drive. The user of the site will select a folder, input minimum GPA, a comma-separated list of universities, and a list of keywords (comma-separated). If a filter is left blank then it is not filtered by that parameter. I want the output to be a google sheet that pulls the following information from the resume; Full Name, phone number, email address, GPA, University(s), keywords, and a link to the specific resume. I want the title of this sheet to include the time of the filtering for sorting purposes. For error treatment if the filtering ai cannot find information then leave it blank. I want two sets of code, a front end with the file input, the three filter boxes and a submit button. Lets also make it green and gold for William and Mary colors. I also need the back end code to have the filtering systems that do as follows: 

Parse each resume and check:
If the GPA meets or exceeds the threshold.
If the resume mentions any of the listed universities (case-insensitive match).
If the resume contains any of the listed keywords (case-insensitive match).

Produce both sets of code along with Google cloud APIs I must activate."

This produced both necessary codes and with a couple tweaks to the code outputted a working site that can be seen here. 

https://script.google.com/macros/s/AKfycbxRTu8sSpwH7BWNHZe2h7H2Jhs9kcMhkhNvCa3qbBxTAYf-5jMI_7OvTxZeMr4R4ce_/exec

*Authentication*
Contact this email for permission to use: drew.messick03@gmail.com



*What Next?*
As AI continues to transform the hiring landscape, understanding how resume scanners shape access to opportunities is more critical than ever. Looking forward, organizations will need to adopt more ethical AI practices, invest in explainable tools, and ensure human oversight in automated hiring. With the rise of regulations and increased public awareness, the future of AI in HR will demand both innovation and responsibility.

*Relevance to the Real World*
- Artificial Intelligence is transforming a lot of the world that we live in today, and many aspects of the business world. Specifically, companies have begun to incorporate AI into how they source, evaluate and hire talent. For prospective candidates looking for job opportunities, and specifically for MSBA students, being able to understand how the processes work is not only intellectually relevant, but practically urgent.
- Companies now receive thousands of applications per role, so they have begun to use Applicant Tracking Systems (ATS), which are powered by AI and machine learning algorithms, to parse and screen candidates’ resumes. Applicant Tracking systems filter resumes based on keyword matching, experience patterns and degree requirements. Now, candidates have to alter their resumes to best pass AI screenings.
- This raises some ethical concerns as people begin to question if AI can faily determine who is the “best fit”? What kind of safeguards exist against discrimination? What kind of data was the model trained on?
- As many of us look for jobs, it is extremely important to understand and know how to best market yourself, to increase your chances against AI screenings

**Article/Study**

*Title*: Using Artificial Intelligence for Hiring Talents in a Moderated Mechanism

*Authors*: Muhaiminul Islam, Md. Mahbubur Rahman, Md. Abu Taher, G. M. Azmal Ali Quaosar & Md. Aftab Uddin

*Summary*: This study explores why AI adoption in employee recruitment remains low in developing countries, focusing specifically on Bangladesh. Using an extended Unified Theory of Acceptance and Use of Technology (UTAUT) framework, it examines key behavioral and contextual factors influencing AI use, including performance expectancy, facilitating conditions, hedonic motivation, and technology complexity. The study also considers demographic moderators such as age, gender, experience, and voluntariness.

*Methodology:* The paper uses a cross-sectional survey of 270 HR professionals in Dhaka and Chattogram that was analyzed using a Partial Least Squares Structural Equation Modeling (PLS-SEM) and a Necessary Condition Analysis (NCA).

*Key Findings*:
- Significant predictors of intention to use AI: Performance expectancy, facilitating conditions, and hedonic motivation.
- Non-significant predictors: Effort expectancy, social influence, and technology complexity.
- Actual AI usage: Driven by intention to use, facilitating conditions, effort expectancy, and hedonic motivation.
- Moderating effects: Only gender had a significant effect (moderated the link between effort expectancy and intention to use).
- NCA findings: Performance expectancy is a necessary condition for intention to use; intention is a necessary condition for actual use.

*Implications*: 
- HR professionals should focus on performance benefits and enjoyable user experiences to drive adoption.
- Gender-sensitive training may help address effort-related adoption barriers.

**Responsible AI Considerations:**
As we examine the use of AI in Human Resources—specifically, resume screening tools—we recognize the importance of designing and evaluating these systems with responsibility, transparency, and fairness at the core. Key responsible AI principles we considered include:
-  ***Fairness and Bias Mitigation:*** AI-driven resume scanners may inadvertently learn and perpetuate historical biases present in hiring data (e.g., gender, race, or educational background). Our project explores how training data, feature selection, and model design can introduce bias—and how techniques like auditing, de-biasing, and algorithmic fairness checks can help mitigate it.
-  ***Transparency and Explainability:*** Resume scanning tools are often "black boxes" to applicants. We advocate for models that offer explainable outputs, so hiring teams understand why certain resumes are filtered or ranked. Transparency is essential not only for building trust, but also for compliance with evolving AI governance regulations.
-  ***Accountability:*** Decisions affecting a candidate’s employment opportunities should never be made solely by machines. We emphasize the importance of maintaining a human-in-the-loop approach, where AI augments rather than replaces human judgment. Additionally, clear documentation of model limitations and decision processes should be required.
-  ***Privacy and Data Security:*** Resume scanners handle sensitive personal data. It is critical that these systems comply with data protection standards (like GDPR or CCPA), ensuring data is used ethically and securely. We also explore the importance of data minimization and proper anonymization techniques in training and evaluating AI models.
-  ***Accessibility and Inclusion:*** AI systems should be designed to accommodate diverse applicant profiles. This includes recognizing non-traditional career paths, varied resume formats, and different linguistic or cultural expressions of skills and experience.

*Reference List:*
1. Using Artificial Intelligence for Hiring Talents in a Moderated Mechanism: https://fbj.springeropen.com/articles/10.1186/s43093-024-00303-x

*Additional Resources:*
1. ChatGPT: https://chatgpt.com/
2. Faker Python Package Documentation: https://faker.readthedocs.io/en/master/
3. Backround Info: https://fitsmallbusiness.com/ai-hiring-trends-and-statistics/
4. More Backround Info: https://www.resumebuilder.com/7-in-10-companies-will-use-ai-in-the-hiring-process-in-2025-despite-most-saying-its-biased/

**Graphics**
![Screenshot 2025-04-09 180524](https://github.com/user-attachments/assets/5de61952-8736-4d93-a390-63083958033f)

![Screenshot 2025-04-09 180821](https://github.com/user-attachments/assets/58aa7c4c-c7ea-4340-8c7b-cd5541448a3b)


