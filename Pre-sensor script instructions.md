# Creating a Pre-Sensor Script for Firewall CI Identification

The full text of the original script could potentially be subject to
copyright restrictions. Therefore, these instructions describe how to
create the script directly in your ServiceNow instance.

## Instructions

1.  In the **Pattern Pre/Post Scripts** table
    (`sa_pattern_prepost_script`), find the script **Update manufacturer
    and model details**, which is part of the **Firewall Audits and
    Reporting** application.
2.  Copy the contents of this script into a new Pre-Sensor script.
3.  In the copied script, replace `cmdb_ci_firewall_device` with
    `cmdb_ci_ip_firewall`.
4.  Associate the new script with your new pattern.

## If the Firewall Audits and Reporting application is not installed

You may be able to use a similar script as a starting point. Look for
other scripts whose names contain the word **model** and that call the
global Script Include `MakeAndModelJS`.

The exact script and required modification may differ, so check that the
selected script performs the same manufacturer and model resolution
before using it.
