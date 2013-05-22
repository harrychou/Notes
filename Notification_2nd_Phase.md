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

* Is it a separate notificaiton or just an attachment?
	- Example: every quarter, a ED is sent out to a specific market, in specific frequent
* Where can I find a sample doc?
	- no, very static information, ... Canada, average variable plan ... 
* Should we save it in LaserFiche? Not associate with customer? Or, each customer got a separate copy?

Reject Notice

* When do we reject? 
	- Utility reject
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

 