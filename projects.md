---
layout: default
title: Projects
permalink: /projects/
---

# Data Science Projects

Here's a collection of my data science projects showcasing different techniques, tools, and domains.

{% for project in site.projects %}
## [{{ project.title }}]({{ project.url }})

**{{ project.description }}**

- **Tech Stack**: {{ project.tech_stack }}
- **Duration**: {{ project.duration }}
- **Status**: {{ project.status }}

{{ project.excerpt }}

[View Project Details]({{ project.url }}) | [GitHub Repo]({{ project.github_url }})

---
{% endfor %}

## Project Categories

- **Machine Learning**: Predictive modeling and classification
- **Data Analysis**: Statistical analysis and hypothesis testing  
- **Visualization**: Interactive dashboards and reports
- **NLP**: Natural language processing projects
- **Time Series**: Forecasting and temporal analysis 