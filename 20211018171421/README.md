# Site Reliability Engineering (SRE): The Big Picture 
 
## Introducing SRE 
 
- SRE teams focus on *automation* *risk reduction* and *handling failures* 
- SRE process requires *blame free post mortem* investigations into problems 
- Address conflicts between dev and ops teams. 
 
## Automation and Eliminating Toil 

- **Toil**: Repetitive, low-value work that reduces high-value time
 
- Restricting toil to 50% (-google)  
  - Example 33% toil On Call Rotation
    - Week 1: Primary On Call (Toil)
    - Week 2: Secondary On Call (Toil)
    - Weeks 3-6: Strategic + (IM/Email/Overflow on call Toil<=17%)
    - Total Toil: 50%
- Identifying areas for automation help eliminate toil 
 
- **Benifits of Reducing Toil** 
  - Increased Productivity
  - System Reliability and availability 
  - Toolset Standardization
  - System simplification
  - Culture of automation  
 
## Service Levels, Monitoring and Alerting 
 
**Service Level Objectives (SLO)**
- Define threshold before action is required
- Agreed between SRE, stakeholders, dev team, and business product owner 
- Need to be *achievable* 
 
**Service Level Indicators (SLI)** 
- Availability
  4800/5000 requests = 96% successful
- Latency 
  Of 5000 requests: (80% within 0.5s)
    4000 within 0.5s 
    600 within 2s 
    300 within 5s 
 
**Service Level Period (SLP)** 
- Period SLOs cover
- Recommended to be 28days 
 
**Four Golden Signals of SLIs** 
1. Latanency: Processing time
1. Traffic: length of message queue 
1. Errors: request failures 
1. Saturation: CPU/Memory utilization and/or Network bandwidth
 
**Effective Alerts** 
- Precision: Only trigger on singificant events 
- Recall: Trigger on all significant events 
- Detection time: Time to trigger an alert 
- Reset Time: time to stop alerting  
 
## Incident Management: On-call and Postmortems  

**Incident Model** 
- Triage: Get back to an *acceptable state* ASAP (exmaple: Add compute power)
- Examine: Understand the problem (Metrics and dashboards)
- Diagnose: Find the cause of the problem 
  - Use some anylitical tools to generate a short list of casues.
    - *What* is it doing?
    - *Why* isn't it doing what it should? 
    -*Where* are resources going? 
    - *When* did it start?
- Test: Narrow down the short list with testing (examples make HTTP requests, run tracroute)
- Cure: Document and apply the fix 

