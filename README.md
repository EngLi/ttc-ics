# ttc-ics

This Excel document includes the method of how to estimate the Time-To-Compromise for the MITRE ATT&CK Techniques in the ICS domain. 
Workflow:
1. Identify the ICS product type and category of vulnerability for the technique by using sheets "Mitre ICS ATT&CK Techniques" and "Mitre Asset mapping".
2. Filter the dataset in "ICS Vulnerability Dataset" according to u_new_cat and u_product_type. This will give the value of v (# of vulnerabilities of the component for that attack).
3. Go to tab "Available exploits (m)" for m (#exploits readily available for that category).
4. Calculate the average value of Base CVSS v2 and Exploitability CVSS v3 for the ICS product type and category of vulnerablity as found in sheet  "Mitre ICS ATT&CK Techniques".
5. The last parameter that needs to be calculated in the MTBV, an example is provided in sheet "MTBV Example".
6. Populate the sheet "Estimate ICS-TTC" with the 5 calculated parameters to estimate the TTC-ICS values.

**References:**


ICS Vulnerability dataset: R.J. Thomas and T. Chothia. (2020) "Learning from Vulnerabilities - Categorising, Understanding and Detecting Weaknesses in Industrial Control Systems" in: Katsikas S. et al. (eds) Computer Security. CyberICPS 2020. Lecture Notes in Computer Science. Springer, Cham. (https://uob-ritics.github.io/learning-from-vulnerabilities/) 

MITRE ATT&CK ICS Techniques (https://attack.mitre.org/techniques/ics/)
