# TSRC Vulnerability Disclosure Program

TCL highly values the security of its products and services, and is committed to developing secure and reliable products and ensuring user privacy protection. In the meantime, we’ve realized that security researchers play an important role in protecting TCL’s products and consumers, which is why the **TSRC (TCL Security Response Center) Vulnerability Disclosure Program** (hereinafter referred to as the Program) is developed. The Program provides a secure channel for researchers to report security issues of the Company and offers effective measures to triage and mitigate the security vulnerabilities. We are truly grateful to the researchers who followed the practice of responsible disclosure and did not disclose the vulnerabilities prematurely during the time required for issue resolution. Premature public disclosure of the vulnerabilities will put TCL users at higher risks. If you have identified any security vulnerabilities or issues in any domain names that belong to or relate to TCL, you are advised to report the vulnerabilities in the website of TSRC.

To protect our users, TCL will not disclose, discuss or confirm any security issues before a full investigation is completed with available updates.

Before you get into the details of the Program, please take a close look at the policies, terms, and conditions of the Program. If you disagree with the policies or terms of this program, you can exit the program and we will stop providing relevant services. If you continue to stay in the program, it means you fully understand and accept the following policies and terms.

---

## Responsible Disclosure - Policy

When reporting a security vulnerability to TCL, we ask that:

- You give us reasonable time to investigate and mitigate an issue you report before making any information contained in the report public or information shared with 3rd parties.
- You do not exploit a security issue you discover for any reason. This includes demonstrating additional risk, such as attempts to compromise sensitive company data or probing for additional issues.
- You do not intentionally violate any other applicable laws or regulations.
- You do not violate any privacy rules, privacy regulations, or cause disruptions to others including, but not limited to, unauthorized access to or destruction of data and interruption or degradation of our services.
- You read, agree and align with TCL Company Privacy Policy.
- You read, agree and adhere to our Responsible Disclosure Terms & Conditions.

### Disclosure Timeline
Once TCL receive the vulnerability report, we will provide an initial response to reporters within 3 working days, and provide our analysis on the vulnerability including whether we have verified that the reported vulnerability is an issue as soon as possible, of which the process may take several days or even weeks depending on the complexity and impact of the vulnerability. Once verified, TCL will work with the relevant internal teams and external partners to mitigate the vulnerability, develop product fixes and prepare appropriate content ahead of disclosure.

### Application for CVE IDs

TCL is the world's 4XXth CVE Numbering Authority (CNA). We can help security researchers who report vulnerabilities in TCL CNA Product List apply for CVE IDs. Security researchers can send their applications to security@tcl.com. The TCL SRC will review their vulnerability reports in line with CVE requirements. If level of the vulnerability is considered to be high or above, the TCL SRC will help the researchers apply for CVE IDs. For details, please read the CVE ID Submission Instructions.

### The vulnerability scope
for the specific scope of vulnerability that TCL will handle, please refer to the link: [TCL Smart Terminal Vulnerability Reward Rules](https://github.com/TclSecLab/CNA/blob/main/TCL%20Smart%20Terminal%20Vulnerability%20Reward%20Rules.md)

### Out of scope

#### Code and Data Protection:
Lack of certificate pinning;
Transmission of sensitive data in URL/request body under TLS protection;

User data stored on external storage without encryption (excluding APP logs containing sensitive information and user data committed to encrypted storage);

Application lacks code obfuscation protection;

APK can be repackaged;

APK contains hardcoded or recoverable keys;
Sensitive data protected by the application’s private directory;
Lack of binary protection controls in Android applications;
Application sets allowBackup to True;

#### Low-Impact DoS:
Sending malformed intents to exported components, resulting only in application crash;
Excessive resource requests leading to browser crash;
Local DoS attack that can be resolved by simply restarting the application;
Temporary framework restart；

#### others:
Application can access data within the scope of the granted permissions after obtaining them;
Runtime hacking attacks using tools such as, but not limited to, Frida/Appmon (possible only in a jailbroken/rooted environment);
Phishing attacks with low level of deception;
Reports too simple to reproduce the vulnerability;
Exploits with extremely strict conditions, high attack cost, and low potential impact/damage;

---

## Responsible Disclosure - Terms & Conditions

- If you inadvertently or intentionally access TCL and its affiliates’ proprietary customer, employee, or business-related information during your testing, the information must not be used, disclosed, stored, or recorded in any way. Access to any such data must be declared as part of your vulnerability report.
- By submitting information about a potential security vulnerability, you are granting TCL a worldwide, permanent, royalty-free, non-exclusive license to use your submission for the purpose of addressing security vulnerabilities in TCL or its affiliates’ products and services. We will respond to your report on TSRC, acknowledge the receipt and update you on our progress. Also we will continue to follow up on the issue until it is resolved. You can check the latest status of the vulnerability reports you submitted by logging into the official TSRC website. This allows you to keep track of the progress until we complete the fixes and close the vulnerability report.  
  **Website:** https://src.tcl.com/
- By submitting a security vulnerability report, you affirm that you have not previously disclosed the security vulnerability to anyone other than TCL. Absent TCL prior written consent, any disclosure outside of this process would be a violation of the terms & conditions of the Program.
