# Project For EECE512 - Information Security

## Do Developers Protect Your Password: A Tool to Detect Password Leakage in Android Applications

Password Leakage in Android Applications is a serious concern to many users. There are papers focus on detecting applications which compromise user privacy, but few of them consider the facts that vulnerabilities of benign applications also lead to password leakage. For example, some applications send out user passwords in plaintext to the Internet, which is vulnerable to Man-in-the-middle attack. 

To deal with this issue, in our project, we developed a tool based on static taint analysis (using FlowDroid) to automatically detect password leakage and provide information for developers to fix the vulnerability. For this specific problem, we provided a list of possible sources (where passwords are retrieved), sinks (where passwords are sent out to the Internet) and conversion methods (what developers should use to protect passwords). We also extend the workflow of FlowDroid so it is forced to find the paths containing the conversion methods. 

To evaluate our proposed method, we tested on 50 applications selected from Top 1,000 applications on Google Play. The result shows that only a little number of applications protect user passwords.
