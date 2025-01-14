---
name: Spring4Shell
severity: high
cvss-score: 9.8
cvss-vector: CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H
cwe-id: ''
cwe-name: ''
compliance: {}

---            

A remote code execution vulnerability (RCE) allows the attacker to execute arbitrary code and operating system commands on the server. In the worst-case scenario, the attacker will be able to fully compromise the server, extract sensitive data, modify the application contents or delete data.

The Spring4Shell RCE vulnerability (CVE-2022-22965) can be easily exploited if the target is running the vulnerable version of the application using Tomcat as a WAR deployment.

## How to fix

{% tabs spring4shell %}
{% tab spring4shell generic %}
To fix the Spring4Shell vulnerability, you need to update all instances of the Spring Framework to version 5.3.18 and 5.2.20, or above, and the Spring Boot (depends on the Spring Framework) to version 2.5.12 and 2.6.6, or above.

Please bear in mind that one of the payloads required to identify this vulnerability might cause the web server logs to become unavailable. Restarting the server fixes this problem.
{% endtab %}

{% endtabs %}
