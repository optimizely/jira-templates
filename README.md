# jira-templates
Repository to hold templates for descriptions of various types of JIRA tickets (Bugs, Features, etc.)

## Usage
- To add a default template for a specific task in your project: Add `/<project>/<taskType>.txt`
- To add a default template for your project: Add `/<project>/default.txt`
- To add a default template for a specific JIRA task type: Add `/default/<taskType>.txt`
- To add a default template for all projects and all task types: Add `/<project>/<taskType>.txt`

### Need Help?
- Ping Dae-Ho or Asa

## Specificity
The template with the most specificity will be used over the more generic template. A specific project wins over a specific task type.

### Examples
- If `/WEB/Bug.txt` is defined, then it will be used for all Bugs under WEB.
- If `/WEB/default.txt` and `/default/Bug.txt` are defined then `/WEB/default.txt` will be used for all Bugs under WEB.
- If none of the following are defined: `/WEB/Bug.txt`, `/WEB/default.txt`, `/default/Bug.txt`, then `/default/default.txt` will be used for all Bugs under WEB.

Note: This is a public repository

