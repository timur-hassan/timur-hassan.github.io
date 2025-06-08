---
layout: default
title: Home
---

# Welcome to My Data Science Portfolio

Hello! I'm a data scientist passionate about extracting insights from complex datasets and building machine learning solutions that drive business value.

## What I Do

- **Machine Learning**: Building predictive models and classification systems
- **Data Analysis**: Exploratory data analysis and statistical modeling  
- **Data Visualization**: Creating compelling visualizations and dashboards
- **Business Intelligence**: Translating data insights into actionable recommendations

## Featured Projects

{% for project in site.projects limit:3 %}
- [{{ project.title }}]({{ project.url }}) - {{ project.description }}
{% endfor %}

[View All Projects](/projects/)

## Skills & Technologies

**Programming Languages**: Python, R, SQL  
**Machine Learning**: Scikit-learn, TensorFlow, PyTorch  
**Data Tools**: Pandas, NumPy, Matplotlib, Seaborn  
**Databases**: PostgreSQL, MongoDB, SQLite  
**Cloud Platforms**: AWS, Google Cloud Platform  
**Visualization**: Tableau, Power BI, Plotly, D3.js  

## Get In Touch

I'm always interested in discussing new opportunities and data science challenges.

- **Email**: [your.email@example.com](mailto:your.email@example.com)
- **LinkedIn**: [linkedin.com/in/yourlinkedin](https://linkedin.com/in/yourlinkedin)
- **GitHub**: [github.com/yourusername](https://github.com/yourusername)

[Download Resume (PDF)](/assets/resume.pdf) 