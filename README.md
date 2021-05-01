# IntelligentProcessLifecycle
The Intelligent Process Lifecycle of Active Cyber Defenders

## Description
This github hosts the poster related files of false positive and error categories in security operation services. The goal is to define an open source reporting standard for Security Operation Center reports. 

This information was first presented at FIRST 2020, the video is available here: https://www.youtube.com/watch?v=pR02cZlPakU

# Continuous Improvement metrics for integrity or technical security compliance monitoring
KPI | Explanation | Target Value | Owner | Risk Type
 :-------------------------- |:----------------------------------------------------| :----- :---------------- :----------------:
 Number of legitimate violations authorized by change | This value reflects events which usually are classic false positives, where all official change processes were correctly followed but the SOC was not included in the process and therefore could not prevent the false alarm
 | < 10 % | Compliance | Endogenous
 Number of configuration errors in baseline | This value reflects what system configurations (or even configuration templates) needs improvement. | < 10 % | Compliance/ Operational | Endogenous
 Number of Limitation in verification products found | If too many of these events were created by configurations, the causing tool should be questioned. | < 5 % | Compliance/ Operational | Endogenous
 Number of activities with no change required | There seems to be a mismatch between the defined security scope and the verified security scope. Gaps should be verified | < 5 % | Policy | Endogenous
Number of unauthorized changes without legitimate cause | Very high numbers → Security process and IT process integration needs rework; Very low numbers → The configurations aren‘t detecting or you are safe | it depends :) | Policy | Endogenous
Number of changes without formal changes | Number of legitimate violation with missed change documentation is highlighting where the SOC had no chance of automating false alerts, as well as where employees are not complying to formal processes. | <5% | Policy/Compliance | Endogenous

# Continuous Improvement metrics for vulnerability management
KPI | Explanation | Target Value | Owner | Risk Type
 :-------------------------- |:----------------------------------------------------| :----- :---------------- :----------------:
Number of delays due to unreasonable SLA | If this value is high very often, correlated to the applications you are running you might be able to impact either SLA or policy documents | 0 | Operational/ Contractual | Exogenous
Numbers of delays due to resource problems or Average # of days delays due to resource problems | If this happens to often it can illustrate how your staff management is impacting the quality of security services. If occuring too often a risk entry is important | 0 | Contractual | Endogenous/Exogenous
Numbers of installed patch on time | This is the goal. If it can’t be reached too often policies or failing reasons should be reviewed | >80% | Counter-Party/ Contractual | Exogenous
Number of blind spots identified | Any time a detection can not be created this should be tracked, possibly by creating risk entries. | < 5% | Operational/ Contractual | Endogenous/Exogenous
Number of context of exploitability not given | Very high numbers → You might not be getting honest responses or your threat identification process is faulty | it depends :) | Counter-Party/ Contractual | Exogenous 





## Authors and acknowledgment
This poster was created by [Desiree Sacher](http://www.twitter.com/d3sre) with sponsorship for the artwork by layer9solutions.de


## Licence
This poster was published under Creative Commons BY License: https://creativecommons.org/licenses/by/4.0/

