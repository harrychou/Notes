# Notification 2nd Phase Design Note

Scope:

* UI	
  - Notification Setup
  - Reporting
  - Health Monitoring
* New Notifications
  - Plan Change Confirmation
  - Environment Disclosure
  - Reject Notice
  - RAF-MX 
  - RAF-CNE
  - SocialSale Email-to-Friend
  - <del>Customer Survey</del> in Jamie's doc, but not estimate
  - <del>Renewal Notification</del> in Jamie's doc, but not estimate
* Error Handling / Monistoring
* Other/Cross-Cut features
  - Segmentation
* To Discuss
  - Push/Pull for each notification type?
  - Remote Start/Stop services
  - Unsubscribe enhancement
  - Pause/Stop/Continue notifications

## UI

Josephine working on it

## New Notification Types

Plan Change Confirmation

* Which Plan Change Confirmation
	- trigger: internal admin
	- push event from Internal Admin 
* Which App initiate the notification?
	- Internal Admin
* same work flow as confirmation email?
* We don't want to resend the welcome packets for plan change (o)
	- need to let call center know plan change is going to send out Welcome packet
	
Environment Disclosure (ED)

* What is the existing process?
  - Currently, it is all manual that James creates a list of recipients/addresses from Siebel (?) based on the market. Then, he gives the list and the EDS document to Fulfillment team to send it out to all customers in the list.
* New Process
  - I think the new process should be for James to ad-hoc (or pre-defined) pick a market (or market hierarchy level) and also upload the EDS document (see the example above). Then, he can push a button and the list will be retrieved from Siebel or SMBDB and notification tasks generated to be processed.
* Is it a separate notificaiton or just an attachment?
	- right now it is always paper letter
  - in the future, we might want to support digital email (html email or attachment?)
* Where can I find a sample doc?
	- very static information, ... Canada, average variable plan ... 
  - see C:\Users\c00522\Desktop\Working Doc\_Notification_PhaseII\MECO Information Disclosure Label 201304.doc
* Should we save it in LaserFiche? Not associate with customer? Or, each customer got a separate copy?
  - we don't have to, since we've saved msg file already

Reject Notice

* When do we reject? 
	- Utility reject
  - we know it is status 55
    * how about 56
  - what previous statuses can become 55
    * only 50?
    * how about others (Siebel processing error?)
* Which apps are involved? Who initiate the process?
* Which Status signals reject?
	- 55 (Enrollment Reject)
* Reject letter can be for currect customer
	- That can result to a different reject letter 

RAF

* Samples
	- after 30/90 days, send out a notice

Social Sale

* Email to friends 
* Just a email tool

## ERCOT

* Credit Check Notification
* Contract Generation Issues?
* This is OK

## Others

Segmentation of Customer

Error Hadling

Servicing Renewal Notification

* Renewal Stuff, at the end of Renwal Segmentation, there will be notifications
* 




















































-- End of File --

 