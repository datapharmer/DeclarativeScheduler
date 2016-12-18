# DeclarativeScheduler
Declarative Scheduler - use the reporting engine and subscribe feature to update records in report on a daily/weekly/monthly schedule


- Create a report with the record id in column 1 and a datetime field in column 2
- Add the filters you like
- Click subcribe. Then select a custom action. Then Declarative Scheduler (make sure to turn off the salesforce1 notification
- Set up when you would like these records to update and then schedule away
- On the scheduled time the datetime field will be updated. So set up a process builder to fire when that field changes. And voilla you have a repeating schedule. 

Notes:
-It works off super batch apex so you can change the batch size in custom settings
- Has been tested to work on reports of up to 50,000 records. Don't go larger of Salesforce CPU times out
- It's built to be generic so works across all obejects - but you should add in your own datatime field. 


Todo:
- Proper test classes
- Instructions
- Testing
- Guidelines and examples


Version 0.1
<a href="https://githubsfdeploy.herokuapp.com/app/githubdeploy/dthowell/DeclarativeScheduler">
<img  class="alignnone size-full wp-image-1966" src="https://andrewfawcett.files.wordpress.com/2014/09/deploy.png?w=820" alt="deploy">
</a>




And a quick managed package link:
https://login.salesforce.com/packaging/installPackage.apexp?p0=04t6F000000Bt1N

