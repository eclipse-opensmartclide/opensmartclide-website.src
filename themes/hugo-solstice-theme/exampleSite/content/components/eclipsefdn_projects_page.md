---
Title: Eclipse Foundation Projects Page
hide_sidebar: true
---

Using the **eclipsefdn_projects** shortcode in order to generate a list of projects that is pulled from the projects.eclipse.org API.

## Parameters:

- **templateId:** string | The mustache template to use
- **url:** string | Url of the PMI endpoint to be using
- **classes:** string | Classes for the block
- **display_categories:** bool | true or false
- **categories:** string | Path to the json file containing the projects categories


## Examples:

Following list of projects has been filtered to display "Cloud Development Tools" projects:

{{< eclipsefdn_projects 
    templateId="tpl-projects-item"
    url="https://projects.eclipse.org/api/projects?working_group=cloud-development-tools"
    classes="margin-top-30"
    display_categories="true"
    categories="/js/featured-projects-categories.json"
>}}

{{< grid/div isMarkdown="false" >}}
    <script type="text/javascript" src="/js/eclipsefdn.projects.js"></script>
{{</ grid/div >}} 