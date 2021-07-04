# IntelligentProcessLifecycle
The Intelligent Process Lifecycle of Active Cyber Defenders

## Description
This github hosts the poster related files of false positive and error categories in security operation services. The goal is to define an open source reporting standard for Security Operation Center reports. The hereby published KPIs are focused on creating statistics relevant for continuous improvement of operational cyber defense tasks.

This information was first presented at FIRST 2020 together with [Eireann Leverett](https://github.com/blackswanburst)(who injected his experience in regards to risk management), the video is available here: https://www.youtube.com/watch?v=pR02cZlPakU

# Continuous Improvement metrics for integrity or technical security compliance monitoring
KPI | Explanation | Target Value | Owner | Risk Type | Business Impact | Motivating Example
 :-------------------------- |:----------------------------------------------------| :----- |:---------------- |:----------------:|:------|:-----|
 Number of legitimate violations authorized by change | This value reflects events which usually are classic false positives, where all official change processes were correctly followed but the SOC was not included in the process and therefore could not prevent the false alarm | < 10 % | Compliance | Endogenous | Governance Risk | Officially approved change to Apache changes configuration format, and detection tools alert on the change.
 Number of configuration errors in baseline | This value reflects what system configurations (or even configuration templates) needs improvement. | < 10 % | Compliance/ Operational | Endogenous | Change and Compliance Management Risk | The baselines for configuration templates were taken from development instead of production systems.
 Number of Limitation in verification products found | If too many of these events were created by configurations, the causing tool should be questioned. | < 5 % | Compliance/ Operational | Endogenous |  SOC Operational risk | Snort rules can't be scoped narrowly to detect the change we're interested in, but if they're given wider scope, produce false positives.
 Number of activities with no change required | There seems to be a mismatch between the defined security scope and the verified security scope. Gaps should be verified | < 5 % | Policy | Endogenous | Policy-operational mismatch leading to overworked SOC | Sysadmin clears logfiles to save space, which needs no approval, but it triggers an alert in the SOC.
Number of unauthorized changes without legitimate cause | Very high numbers → Security process and IT process integration needs rework; Very low numbers → The configurations aren‘t detecting or you are safe | it depends :) | Policy | Endogenous | Potential intrusion/Prioritise investigation | IIS server has added a user and administrator denies knowledge of event.
Number of changes without formal document | Number of legitimate violation with missed change documentation is highlighting where the SOC had no chance of automating false alerts, as well as where employees are not complying to formal processes. | <5% | Policy/Compliance | Endogenous | Shadow IT Administration Risk | Sysadmin changes configuration of Apache server without formal change management documentation (but it would have been approved).    

# Continuous Improvement metrics for vulnerability management
KPI | Explanation | Target Value | Owner | Risk Type | Business Impact | Motivating Example
 :-------------------------- |:----------------------------------------------------|:----- |:----------------| :----------------:|:------|:-------:|
Number of delays due to unreasonable SLA | If this value is high very often, correlated to the applications you are running you might be able to impact either SLA or policy documents | 0 | Operational/ Contractual | Exogenous | Risk Appetite and Contractual Management teams need to match expectations | Network switches only have two change windows a year and don't get patched, but contracts still punish counter party for unpatched systems
Numbers of delays due to resource problems or Average # of days delays due to resource problems | If this happens to often it can illustrate how your staff management is impacting the quality of security services. If occuring too often a risk entry is important | 0 | Contractual | Endogenous/Exogenous | Operational Risk management | Staff resource problems in some teams delay patching
Numbers of installed patch on time | This is the goal. If it can’t be reached too often policies or failing reasons should be reviewed | >80% | Counter-Party/ Contractual | Exogenous | Cyber Risk Expectation isn't being met | 99/100 windows computers are patched on time, but 1 is considered high risk to patch.

# Continuous Improvement metrics for Log management
KPI | Explanation | Target Value | Owner | Risk Type | Business Impact | Motivating Example
 :-------------------------- |:----------------------------------------------------|:----- |:----------------| :----------------:|:----------------------------------------------------|:----------------------------------------------------|
Number of blind spots identified | Any time a detection can not be created this should be tracked, possibly by creating risk entries. | < 5% | Operational/ Contractual | Endogenous/Exogenous | No visibility on the operational risk register | The Active Directory logs cannot be ingested by the SOC because the identity management teamdoesn't have enough resources.
Number of context of exploitability not given | Very high numbers → You might not be getting honest responses or your threat identification process is faulty | it depends :) | Counter-Party/ Contractual | Exogenous | Potentially Poor Risk Acceptance Practices | The technical engineering team defer every patch as unexploitable to avoid applying resources.


My other continuous improvement KPIs for security monitoring can be found here: https://github.com/d3sre/Use_Case_Applicability 


## Authors and acknowledgment
This poster was created by [Desiree Sacher](http://www.twitter.com/d3sre) with sponsorship for the artwork by layer9solutions.de


## Licence
This poster was published under Creative Commons BY License: https://creativecommons.org/licenses/by/4.0/

