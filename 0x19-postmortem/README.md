
# My First Postmortem: The Case of the Overloaded Database

## Introduction

Picture this: It's a sunny Friday morning, and you're sipping your coffee, ready to dive into your tasks for the day. Suddenly, your phone buzzes with an alert. The e-commerce platform is down! Panic ensues, but fear not! This postmortem will take you through the thrilling journey of how we identified and resolved this catastrophe.

## Issue Summary

**Duration of the Outage:**
- Start Time: June 7, 2024, 10:00 AM (WAT)
- End Time: June 7, 2024, 12:00 PM (WAT)

**Impact:**
- The company's main e-commerce platform was down for two hours.
- Users experienced a complete inability to access the site, resulting in lost sales.
- Approximately 80% of users were affected, as the platform was entirely non-functional during this period.

**Root Cause:**
- The outage was caused by a misconfiguration in the database server settings, leading to a cascade failure that brought down the application server.

## Timeline

![Timeline of the Outage](timeline_diagram.jpg)

- **10:00 AM:** Issue detected via monitoring alert indicating high response times and eventual timeouts on the main e-commerce platform.
- **10:05 AM:** Engineers received automated alerts and began investigating.
- **10:10 AM:** Initial assumption was a network issue; network diagnostics were run.
- **10:20 AM:** Misleading path: Network diagnostics showed no issues. Attention shifted to the application server.
- **10:30 AM:** Application logs reviewed, but no immediate issues found.
- **10:45 AM:** Escalation to the database team after noticing database connection errors in application logs.
- **11:00 AM:** Database team identified misconfiguration in database server settings.
- **11:15 AM:** Database settings corrected, and services began to stabilize.
- **12:00 PM:** Full functionality restored, and all services running normally.

## Root Cause and Resolution

**Root Cause:**
- A recent configuration change in the database server settings inadvertently set the maximum connections limit too low. This led to the application server being unable to establish new database connections as user requests surged, causing the application server to crash.

**Resolution:**
- The database settings were corrected to increase the maximum connections limit.
- The application server was restarted, which allowed it to reconnect to the database properly.
- Continuous monitoring confirmed that the system stabilized and returned to normal operations.

## Corrective and Preventative Measures

**Improvements:**
- Implementing more stringent review processes for configuration changes.
- Enhancing monitoring to detect configuration issues more quickly.
- Conducting regular load testing to ensure the system can handle high traffic volumes without failing.

**Tasks:**
1. **Patch Database Server:** Review and apply patches to prevent similar issues.
2. **Add Monitoring on Database Connections:** Set up alerts for database connection limits.
3. **Enhance Configuration Review Process:** Implement a mandatory peer review for all configuration changes.
4. **Conduct Load Testing:** Schedule regular load testing to simulate high traffic scenarios and identify potential issues.
5. **Document Procedures:** Create detailed documentation for configuration changes and emergency response protocols.

## Conclusion

Every cloud has a silver lining, and every outage is an opportunity to learn and improve. By examining the root cause and implementing preventative measures, we can ensure our systems become more robust and resilient. And remember, when in doubt, always double-check those configuration settings!

## Repository Information
- **GitHub repository:** alx-system_engineering-devops
- **Directory:** 0x19-postmortem
- **File:** README.md
