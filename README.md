# Postmortem

> "_The cost of failure is education_"  
  _Devin Carraway_

## How To Use This Repository

1. Carefully read about blameless postmortem culture in this document

2. Copy [postmortem template](TEMPLATE.md) file to a subdirectory with a matching year. Rename template file to match `[month].[system].[event].md` naming convention. Fill in the postmortem report using the structure and guidelines provided in the template. 
Place any additional files such as log files, figures or e-mails into a `[month].[system].[event]` subdirectory. _Take your time and be thorough._ Collaborate with your colleagues or enlist help in order to establish an incident timeline and identify a root cause of the event.

3. When a report has been completed, schedule a postmortem review session with your teammates. It is important to close any ongoing discussions, unanimously agree on the incident root cause, go over lessons learned from the incident, create and assign action items and finalize the state of the report. Remember, an unreviewed postmortem might as well never have existed.

4. Disseminate postmortem results to a wider audience via a monthly newsletter, RnD & Ops Team meeting, 3DS Group, etc.

## Postmortem: Learning from Failure

Incidents and outages are inevitable. When an incident occurs, we fix underlying issues and return services to their normal operating conditions. But unless we establish some formalized process of learning from such incidents, they may reoccur in the future. Left unchecked, incidents can multiply in complexity or even cascade, overwhelming a system and its operators, impacting users and business.

The primary goals of writing a postmortem are to ensure that the incident is documented, that all contributing root cause(s) are well understood, and, especially, that effective preventive actions are put in place to reduce the likelihood and/or impact of recurrence. Writing a postmortem is not punishment — it is a learning opportunity for the entire company.

Postmortems also help to restore confidence and credibility with the users that were impacted by the outage and server as a sort of institutional knowledge that remains within the company for further generation of engineers to learn from.

### When to write a postmortem

The postmortem process does present an inherent cost in terms of time and effort, so be deliberate in choosing when to write one. Some common postmortem triggers are:

* Core services or critical infrastructure downtime
* User-facing systems unavailible beyond a certain threshold 
* Severe performance degradation for prolonged time
* Data loss or data corruption
* Security breach

### Who completes the postmortem?

The delivery team for the service that failed is responsible for completing the postmortem. That team selects the postmortem owner and reviews postmortem when it is ready.

### Establish a blameless culture 

Blameless culture originated in the healthcare and avionics industries where mistakes can be fatal. These industries nurture an environment where every mistake is seen as an opportunity to strengthen the system. When postmortems shift from allocating blame to investigating the systematic reasons why an individual or team had incomplete or incorrect information, effective prevention plans can be put in place. You can’t fix people, but you can fix systems and processes to better support people making the right choices.
By focusing on events rather than the people, postmortems provide significant value.

Blameless postmortems can be challenging to write, because the postmortem format clearly identifies the actions that led to the incident. Removing blame from a postmortem gives people the confidence to escalate issues without fear. It is also important not to stigmatize frequent production of postmortems by a person or team. An atmosphere of blame risks creating a culture in which incidents and issues are swept under the rug, leading to greater risk for the organization 

### No Postmortem Left Unreviewed

When an outage does occur, a postmortem is not written as a formality to be forgotten. Ensure that each completed postmortem is reviewed and added to a repository of past incidents. Transparent sharing makes it easier for others to find it, learn from the postmortem and avoid same or similar mistakes in the future.

Writing a postmortem involves formal review and publication. In practice, teams share the first postmortem draft internally and assess the draft for completeness. Review criteria might include:

* Was key incident data collected for posterity?
* Are the impact assessments complete?
* Was the root cause sufficiently deep?
* Is the action plan appropriate and are resulting bug fixes at appropriate priority?
* Did we share the outcome with relevant stakeholders?

Once the initial review is complete, the postmortem is shared more broadly, typically with the larger audience or on an internal mailing list.

Host postmortem reading clubs, in which an interesting or impactful postmortem is brought to the table for an open dialogue with participants, nonparticipants, and new employees about what happened, what lessons the incident imparted, and the aftermath of the incident. You might even exercise Disaster Role Playing games in which a previous postmortem is being reenacted.

### Learning from Failure 

When an incident occurs, it’s important to evaluate what went wrong, recognize what went well, and take action to prevent the same errors from recurring in the future. Don't be afraid of asking hard questions, get to the root of the problem and see what could have prevented the problem or could be done differently.

Never let the same incident happen twice! Make sure that all your action items have a clear owner assigned to them and a JIRA ticket is created for each such item.
