# JIRA Worklog Extractor

Tool to help extract worklogs from JIRA. The native UI and REST interface for dealing with worklogs is a bit clunky so I wrote
this little tool to help with it.

Currently outputs a CSV table with the projects on the rows, authors on the columns and worked hours in the cells.

# Usage

```
git clone https://github.com/zamoroka/jira-worklog-extractor.git
```

- Copy the `config.json.template` to `config.json` and alter the values.
- Add [API token](https://id.atlassian.com/manage/api-tokens) into the `password` node

To run it:
````bash
php app.php worked-hours-per-day 2020-02-17 2020-02-24
````

# License

MIT License

# Thanks to

Marius Storm-Olsen for his code sample on https://answers.atlassian.com/questions/87961/how-to-get-list-of-worklogs-through-jira-rest-api
