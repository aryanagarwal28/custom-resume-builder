# custom-resume-builder
a tool to make your resume from scratch
Insructions to use:

Download and Install Python:

Ensure you have the last Python version installed. If not, download and install it from Python's official website. For detailed instructions, refer to the tutorials:

Download and Install Google Chrome:

Download and install the latest version of Google Chrome in its default location from the official website.


Ensure you have pip installed, then run:

pip install -r requirements.txt
Configuration
1. Configuring plain_text_resume.yaml
The plain_text_resume.yaml file is crucial as it contains all your personal details and resume content. Follow these steps to configure it properly:

1. Create the File
Create a file named plain_text_resume.yaml in the root directory of your project. This file will store all the necessary details to generate your resume.

2. Define Personal Information
Fill in your personal information. This section includes your basic details and contact information:

personal_information:
  name: [Name]
  surname: [Surname]
  date_of_birth: "[DD/MM/YYYY]"
  country: [Country]
  city: [City]
  address: [Address]
  phone_prefix: "[+Country Code]"
  phone: "[Phone Number]"
  email: [Email Address]
  github: [GitHub URL]
  linkedin: [LinkedIn URL]
name: Your first name.
surname: Your last name.
date_of_birth: Your date of birth in the format DD/MM/YYYY.
country: The country where you live.
city: The city where you live.
address: Your home address.
phone_prefix: Your phone number prefix, e.g., +1 for the USA.
phone: Your phone number.
email: Your email address.
github: Your GitHub profile URL (optional).
linkedin: Your LinkedIn profile URL (optional).
3. Provide Education Details
List your educational qualifications. You can add multiple degrees:

education_details:
  - degree: [Degree Type]
    university: [University Name]
    gpa: "[GPA]"
    graduation_year: "[Graduation Year]"
    field_of_study: [Field of Study]
    exam:
      [Course Name]: "[Grade]"
      [Course Name]: "[Grade]"
      [Course Name]: "[Grade]"
  - degree: [Degree Type]
    university: [University Name]
    gpa: "[GPA]"
    graduation_year: "[Graduation Year]"
    field_of_study: [Field of Study]
    exam:
      [Course Name]: "[Grade]"
      [Course Name]: "[Grade]"
      [Course Name]: "[Grade]"
degree: Type of degree (e.g., BSc, MSc, PhD).
university: Name of the university or institution.
gpa: Your GPA (optional).
graduation_year: The year you graduated.
field_of_study: Your field of study (e.g., Computer Science).
exam: List of courses and grades received. Add or remove entries as needed.
4. List Experience Details
Provide information about your work experience. You can include multiple jobs:

experience_details:
  - position: [Job Title]
    company: [Company Name]
    employment_period: "[MM/YYYY - MM/YYYY or Present]"
    location: [Location]
    industry: [Industry]
    key_responsibilities:
      - [Responsibility Description]
      - [Responsibility Description]
      - [Responsibility Description]
    skills_acquired:
      - [Skill]
      - [Skill]
      - [Skill]
  - position: [Job Title]
    company: [Company Name]
    employment_period: "[MM/YYYY - MM/YYYY or Present]"
    location: [Location]
    industry: [Industry]
    key_responsibilities:
      - [Responsibility Description]
      - [Responsibility Description]
      - [Responsibility Description]
    skills_acquired:
      - [Skill]
      - [Skill]
      - [Skill]
position: Your job title.
company: Name of the company where you worked.
employment_period: The period you worked there (e.g., 01/2020 - 12/2021 or Present).
location: City and country of the company's location.
industry: The industry of the company.
key_responsibilities: List of key responsibilities in bullet points.
skills_acquired: List of skills acquired during this role.
5. Detail Your Projects
Include projects that you have worked on:

projects:
  - name: [Project Name]
    description: [Project Description]
    link: "[Project URL]"
  - name: [Project Name]
    description: [Project Description]
    link: "[Project URL]"
  - name: [Project Name]
    description: [Project Description]
    link: "[Project URL]"
name: Name of the project.
description: A brief description of the project.
link: URL to the project or related resource (optional).
6. Add Achievements
List notable achievements:

achievements:
  - name: [Achievement Title]
    description: [Achievement Description]
  - name: [Achievement Title]
    description: [Achievement Description]
  - name: [Achievement Title]
    description: [Achievement Description]
  - name: [Achievement Title]
    description: [Achievement Description]
name: Title of the achievement.
description: Description of the achievement.
7. List Certifications
Include any certifications you hold:

certifications:
  - [Certification Name]
certification: Name of the certification.
8. Detail Your Language Skills
List the languages you speak and your proficiency levels:

languages:
  - language: [Language]
    proficiency: [Proficiency Level]
  - language: [Language]
    proficiency: [Proficiency Level]
  - language: [Language]
    proficiency: [Proficiency Level]
language: Name of the language.
proficiency: Your proficiency level (e.g., Basic, Intermediate, Advanced).
9. Add Interests
Include your personal interests:

interests:
  - [Interest]
  - [Interest]
  - [Interest]
interest: List your interests or hobbies.
Example plain_text_resume.yaml
An example plain_text_resume.yaml file is provided in the repository to guide you. Copy and modify it according to your personal details.

2. Configuring secrets.yaml
This file contains sensitive information. Never share or commit this file to version control.

openai_api_key: [Your OpenAI API key]
Replace with your OpenAI API key for GPT integration
To obtain an API key, follow the tutorial at: https://medium.com/@lorenzozar/how-to-get-your-own-openai-api-key-f4d44e60c327
Note: You need to add credit to your OpenAI account to use the API. You can add credit by visiting the OpenAI billing dashboard.
Usage
To run the custom resume builder run the python main.py file
