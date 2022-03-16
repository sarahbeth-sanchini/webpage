# FDA Adverse Events - Data Extraction and Analysis

## Introduction

The FDA launched its openFDA project in 2014, which provides the public with access to APIs and raw datasets of adverse events, drug product labeling and recall enforcement reports in several areas. 

Each year, the FDA receives several hundred thousand medical device reports (MDRs) of suspected device-associated deaths, serious injuries and malfunctions. The FDA uses MDRs to monitor device performance, detect potential device-related safety issues, and contribute to benefit-risk assessments of these products.In this project I have pulled all the adverse events data relevant to Straumann. 

**The following steps were performed:**

1.	Download adverse events data from openFDA via API 
2.	Data cleaning and transformation using Python
3.	Uploaded the data to internal Postgres database
4.	Access and host data with SAP Data Warehouse Cloud - available to all Straumann employees
5.	Created SAP Analytics Cloud Dashboard – can be used as template for future dashboards/visualizations

### 1.  Download adverse event data from openFDA

#### **openFDA API overview:**

The openFDA API is a program hosted by the website. They provide the consumer with a method to GET data in a structured format, in this case a JSON is returned. 

Link to datasource:             
[openFDA_database](https://open.fda.gov/apis/device/event/download/)

API call specifications:
- Time Frame: 1991 – Current (2022 Q1)
- Refresh Rate: Quarterly
- The FDA API has the following limitations:
- 120,000 calls/day 
- 1,000 results/call




To make these calls, you can either manually put the URL in the URL address bar in your browser or in this case write a script to do it automatically. 

Example: ![openFDA API call]







<!-- This content will not appear in the rendered Markdown 
You can use the [editor on GitHub](https://github.com/sarahbethsleipnir/webpage/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/sarahbethsleipnir/webpage/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

-->
