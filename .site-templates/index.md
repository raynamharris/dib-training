{# receives 'issues_list', 'labels_to_issues', and 'piggy' #}

# Welcome to the {{config.site_name}}!

This is a collection of examples for software and tools used by the Data Intensive Biology Lab.


{% for issue in issues_list %}
{% if issue.is_frontpage %}

[{{config.issue_title_prefix}}{{issue.title}}]({{issue.output_filename}})

{% endif %}
{% endfor %}

---

## [All examples](examples.md)

---

## [All categories](labels.md)
