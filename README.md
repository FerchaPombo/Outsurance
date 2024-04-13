# Outsurance Data Analytic Research and Plan
Facts :

### Project Goals 
Doing the math (Business modell)
In Germany, 8% identify as LGBTIQ+ - so we have around 6.4 Million people. Let’s say we can reach 5% of them, we have 0.05 * 6.4 Million = 320.000 people.
Let’s say 5% need a therapy per year ==> an average therapy takes 50 sessions with an average cost of 120€ per hour = 5 / 100 * 320.000* 50 * 120€ = 96 Mio €. Personal costs (app developers, marketing, IT-support, …) : 12 * 70.000€ salary per year = 840.000€
Server costs: 10.000€/month * 12 = 120.000€
Total per year: 97 Mio €
Per year and user: 97 Mio € / 320.000 users = 303€/user ==> per month: 25€ / user (average net-salary per employee in Germany: 2.425€/month ==> so we are talking about 1% of your net salary….) 
### Stakeholders

The primary stakeholders involved in the data collection, analysis, and usage within the company are dedicated to upholding user privacy as a core value. All data collected will be treated with sensitivity and confidentiality, accessible only to the company's management team. Following data collection, analysis, transformation, and processing, insights will be leveraged, with continued emphasis on user privacy, to identify areas of concern and promote awareness surrounding mental health, intersectionality, and accessibility, particularly for the queer population in Germany. A key objective of analyzing this data is to ensure that the funding for our services remains accessible to everyone, aligning with our commitment to inclusivity and equity.
After the appropriate data collection, it will be analyzed and shared with the Analytics team for further processing. The results will then be provided to the developers team in concise steps, outlining necessary changes to be made to the interface based on the data collected. Continuous feedback will be provided across different teams within the company to facilitate significant adjustments in the data collection, analysis, cleaning, and visualization processes, aiming for improved results with each iteration. This iterative approach ensures that our platform evolves to better meet the needs of our users over time.

### Discovery:

Users' Needs: Our users are seeking assistance, a sense of community, and tangible results. They require swift and effective access to therapy for mental health improvement. The platform must offer an accessible, user-friendly interface where individuals can easily find the right therapist based on their unique needs, backgrounds, spoken languages, and other demographic factors collected.

Data Requirements: Data will primarily originate from users and therapists, with the database being the target repository. This data will fuel the creation of algorithms designed to provide personalized assistance to individuals based on their specific needs. It's imperative that data collection is conducted with the full consent of each user, prioritizing privacy concerns throughout the process.

Data Quality: Our focus is on obtaining high-quality, personalized data directly from users, avoiding assumptions and nuances that could compromise the integrity of the information. We acknowledge the risks associated with making assumptions on behalf of the company and are committed to mitigating them by ensuring that data collection is accurate, precise, and respectful of user privacy.

The data collected through daily mood assessments and detailed feedback provides valuable insights into users' mental health progression. By tracking users' responses over time, we can quantitatively measure improvements or setbacks in their well-being. Analyzing patterns in users' experiences, accomplishments, and obstacles empowers us to provide tailored support. Additionally, statistics on successful therapist matches, user referrals, and consultation feedback serve as key indicators of platform effectiveness and user satisfaction. Monitoring metrics related to sponsorships and sliding-scale plans allows us to evaluate accessibility and efficacy in reaching economically disadvantaged individuals. Furthermore, tracking the growth of our therapist network informs strategic decisions to sustain and expand our initiatives. Ultimately, these statistics play a pivotal role in guiding decision-making and driving continuous improvement to meet the diverse needs of our users.

### Data Pipeline and Structure

ELT Strategy for Building a Data Pipeline for Outsurance:

ELT, or Extract, Load, Transform, describes the process of integrating data by extracting it from a source, loading it into a target repository, and then transforming it for downstream use, typically in a cloud-based data warehouse.

Locate Your Data Source and Ensure Access:
Data will be sourced from the platform itself through regular questionnaires and feedback collected from users.

Integrate Your Data Sources with Your Cloud Data Warehouse:
Data integration will occur within the chosen cloud data warehouse platform, such as Snowflake or BigQuery.

Build Your Data Models to Transform Raw Source Data:
The Data Analytics team will develop data models to transform raw data into desired statistics as required.

Control Access to Your Data Models:
Access to data models will be carefully managed within the Data Analytics team to ensure privacy and protect user data.

Set Up Orchestrations for Automation:
Automation logic sequences and schedules will be established to trigger data processing automatically.

Implement Data Tests:
Data tests will be created and deployed to identify breakdowns in the data workflow, preventing failures.

Set Up Notifications:
Notifications will be configured to alert designated users of the data pipeline's progress and any issues encountered.

Deploy Data Tables for Downstream Applications:
Once the data pipeline is production-ready, data tables will be shared with downstream applications and users via reverse ETL, allowing them to build visualizations based on a single source of truth - the data pipeline.

#### Detailed Plan for Data Collection and Usage:

Time to Service:

Implement a system that timestamps user requests for mental health support and tracks the time until they receive assistance.
Utilize a centralized database to record and analyze this data, ensuring accuracy and reliability.
Regularly review the time-to-service metrics to identify trends, bottlenecks, and areas for improvement.
Collaborate with the technical team to optimize platform performance and response times based on these findings.
Conduct periodic user surveys or interviews to gather qualitative feedback on their experience with the time to service.
Demographics:

Develop a comprehensive questionnaire to gather demographic information during the user registration process.
Include questions about age, gender, language preferences, cultural background, and socioeconomic status.
Ensure data privacy and security by implementing robust encryption protocols and obtaining user consent for data collection.
Analyze demographic data regularly to identify any disparities in access to mental health services.
Use demographic insights to tailor outreach efforts, content, and support services to better meet the needs of diverse user groups.
Periodically update the demographic questionnaire to capture evolving user demographics and preferences.
Mental Health Improvement:

Integrate regular mood assessments and mental health tracking features into the platform.
Design surveys or questionnaires to measure users' well-being, coping mechanisms, and perceived improvements over time.
Utilize standardized mental health assessment tools to quantify changes in users' mental health status.
Aggregate and analyze data from mood assessments and surveys to track overall mental health improvement trends.
Collaborate with mental health professionals to interpret the data and identify strategies for optimizing user support.
Provide users with personalized feedback based on their mental health assessment results, offering resources and recommendations for improvement.
Primary Health Concern:

Incorporate prompts or questionnaires during user interactions to identify their primary mental health concerns.
Develop a standardized framework for categorizing and analyzing users' primary health concerns.
Train support staff to engage users in conversations about their specific mental health challenges and needs.
Utilize natural language processing (NLP) algorithms to analyze free-text responses and extract key themes and concerns.
Regularly review primary health concern data to identify emerging trends and prioritize support initiatives.
Adjust platform content, resources, and support services based on the identified primary health concerns to better meet users' needs.
Symptom Severity Before and After Treatment:

Implement pre- and post-treatment assessments to measure changes in symptom severity.
Develop standardized assessment tools or surveys to quantify the severity of users' symptoms before and after therapy sessions.
Ensure that therapists are trained to administer and interpret the assessment tools accurately.
Store assessment data securely in a centralized database for analysis and comparison.
Use statistical analysis techniques to compare pre- and post-treatment symptom severity scores and evaluate therapy effectiveness.
Provide therapists with regular feedback on their clients' progress based on the symptom severity data.

### Resources 

[](https://de.statista.com/infografik/27440/anteil-der-befragten-die-ihre-sexuelle-orientierung-wie-folgt-angeben-nach-geburtsjahr/)
[](https://www.psychomeda.de/psychotherapie/was-kostet-psychotherapie.html#:~:text=Je%20nach%20Therapieform%2C%20St%C3%B6rung%20und%20Therapieziel%20betr%C3%A4gt%20die,entspricht%20und%20zwischen%2050%20und%20150%20EUR%20kostet.)
[]( https://de.statista.com/statistik/daten/studie/370558/umfrage/monatliche-nettoloehne-und-gehaelter-je-arbeitnehmer-in-deutschland/)
[](https://de.statista.com/statistik/daten/studie/370558/umfrage/monatliche-nettoloehne-und-gehaelter-je-arbeitnehmer-in-deutschland/)
[How population identifies in germany](https://de.statista.com/infografik/27440/anteil-der-befragten-die-ihre-sexuelle-orientierung-wie-folgt-angeben-nach-geburtsjahr/)
[Data Strategy plan](https://www.phdata.io/blog/data-strategy-framework-healthcare-providers/)
[Data Platform Architecture](https://www.y42.com/blog/data-pipeline-architecture?utm_term=&utm_campaign=Y42+%7C+Performance+Max+%7C+Leads&utm_source=adwords&utm_medium=ppc&hsa_acc=6839813425&hsa_cam=20808672417&hsa_grp=&hsa_ad=&hsa_src=x&hsa_tgt=&hsa_kw=&hsa_mt=&hsa_net=adwords&hsa_ver=3&gad_source=1&gclid=Cj0KCQjw2uiwBhCXARIsACMvIU0vUIGabeqYviUciiA3NXk4DtwFDNUvuoyrqOMmw_vAgxCj6xf3igcaAhFUEALw_wcB)
