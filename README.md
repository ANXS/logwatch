[![Build Status](https://travis-ci.org/LibreIT/ansible-logwatch.png)](https://travis-ci.org/LibreIT/ansible-logwatch)

logwatch
========

Installs and configures logwatch.


Role Variables
--------------

```yaml
logwatch_email_to: "root@localhost"  # Email Address which Logwatch reports to
logwatch_email_from: ""           # Email Address of the sender of reports (default "ansible_hostname"@"ansible_domain")
logwatch_detail: "low"            # The level of detail in the Logwatch report
logwatch_range: "yesterday"       # The default time range for the Logwatch report
logwatch_output: "stdout"         # The output method of the Logwatch report
logwatch_format: "text"           # The format of the Logwatch report
logwatch_cron_time: "daily"       # Cron special time specification nickname - must match with logwatch range!
```

Example
========

    - hosts: example
      roles:
         - { role: kalos.logwatch }


License
-------

MIT

Author Information
------------------

Calogero Lo Leggio (kalos) - http://LibreIT.org
Pjan Vandaele - https://github.com/Ansibles/logwatch
