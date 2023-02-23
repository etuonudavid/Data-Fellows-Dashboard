# Data Fellowship dataset exploration

This is a simple report that contains analysis of the the questionnaires given to the members of a data fellowship community.
It is made up of two datasets - The data fellows survey and the data fellows Bio-data form.

The survey dataset consists of 9 columns:
- Timestamp (The time for filling the form)
- email address (Email of the member)
- Please state your interest of specialization (Area of specialization or job)
- rate your level of proficiency (Beginner to advanced)
- Which of these tools do you have high proficiency in? (data analysis tool the member can use)
- Have you worked on a project or you are currently working on one?
- If you have worked on a report/project or you have a portfolio, kindly include the links
- If you could mentor or guide someone new to a skill, which of these tools would you be much comfortable teaching
- What tool or area would you like to improve yourself on?

The Bio-data form consists of 4 columns
- Email address
- Name
- How many years of Data experience do you have?
- Which one are you? (IS the member a data analyst or a data scientist)


**Cleaning and Transformation were made in the datasets such as**
- Changing of long column names to a shorter column names
- filtering the datasets for only data analysts and data scientists
- some columns were having comma separated entries and these columns were used to create separate tables and the comma separated values were split and used to form new rows while keeping the email field as a foreign key in these tables
- column such as "Have you worked on a project or you are currently working on one?" are meant to be binary but were having other texts in them, this was turned into either a true or false entry
- null values in the "If you have worked on a report/project or you have a portfolio, kindly include the links" were turned into a no as the members did not have a portfolio website

The tables were Joined using the email field and then imported into Power Bi for visualization.

You can download the pdf and the pbix file.
