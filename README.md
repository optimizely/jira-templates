# jira-templates
Repository to hold templates for descriptions of various types of JIRA tickets (Bugs, Features, etc.)

## Usage
- To add a default template for a specific task in your project: Add `/<project>/<taskType>.txt`
- To add a default template for your project: Add `/<project>/default.txt`
- To add a default template for a specific JIRA task type: Add `/default/<taskType>.txt`
- To add a default template for all projects and all task types: Add `/<project>/<taskType>.txt`

## Specificity
The template with the most specificity will be used over the more generic template. A specific project wins over a specific task type.

### Examples
- `/WEB/Bug.txt` would be used for any Bugs created under the WEB JIRA project and will trump all other templates.
- `/WEB/default.txt` will be used over `/default/Bug.txt`
- Lastly `/default/default.txt` will be used if there is not a template defined for the project or task type.

Note: This is a public repository
