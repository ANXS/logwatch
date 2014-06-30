## Ansibles - logwatch [![Build Status](https://travis-ci.org/Ansibles/logwatch.png)](https://travis-ci.org/Ansibles/logwatch)

Ansible role which installs and configures logwatch.


#### Requirements & Dependencies
- Tested on Ansible 1.4 or higher.


#### Variables

```yaml
logwatch_email_to: "root@localhost"  # Email Address which Logwatch reports to
logwatch_email_from: ""           # Email Address of the sender of reports (default "ansible_hostname"@"ansible_domain")
logwatch_detail: "low"            # The level of detail in the Logwatch report
logwatch_range: "yesterday"       # The default time range for the Logwatch report
logwatch_output: "stdout"         # The output method of the Logwatch report
logwatch_format: "text"           # The format of the Logwatch report
logwatch_cron_time: "daily"       # Cron special time specification nickname - must match with logwatch range!
```


#### License

Licensed under the MIT License. See the LICENSE file for details.


#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/ansibles/logwatch/issues)!
