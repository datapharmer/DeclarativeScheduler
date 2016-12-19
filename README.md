# Declarative Scheduler Tool
Declarative Scheduler - use the reporting engine and subscribe feature to update records in report on a daily/weekly/monthly schedule


- Create a report with the record id in column 1 and a datetime field in column 2
- Add the filters you like
- Click subcribe. Then select a custom action. Then Declarative Scheduler (make sure to turn off the salesforce1 notification
- Set up when you would like these records to update and then schedule away
- On the scheduled time the datetime field will be updated. So set up a process builder to fire when that field changes. And voilla you have a repeating schedule. 
<br><br>

# Sample user cases
- A report of all leads over 4 days that have been stuck on a status for 4 days
- Create a task to follow up on all opportunities that have a closed date in the past and no follow up tasks and haven't been modified in the last 7 days
- Send an email on a contacts birthday
- Process mass updates to all data (create a workflow to fire when the triggering field change and then to do the function you want)
- Delay bulk workflow actions into a nightly job
- Let me know yours...

<br>
Notes:
- It works off super batch apex so you can change the batch size in custom settings
- Has been tested to work on reports of up to 50,000 records. Don't go larger of Salesforce CPU times out
- It's built to be generic so works across all obejects - but you should add in your own datatime field. 

<br>
Todo:
- Proper test classes
- Instructions
- Testing
- Guidelines and examples




# Instructions
Install the package below.<br>
<img src="https://lavaboxdeclarativescheduler-dev-ed--c.ap4.content.force.com/servlet/servlet.ImageServer?id=0156F00000Cf6Ko&amp;oid=00D6F000000EMro&amp;lastMod=1482131370000" alt="Right click on the image to save it to your computer." title="Right click on the image to save it to your computer.">

<br><br><br>
<img src="https://lavaboxdeclarativescheduler-dev-ed--c.ap4.content.force.com/servlet/servlet.ImageServer?id=0156F00000Cf6L3&amp;oid=00D6F000000EMro&amp;lastMod=1482131405000" alt="Right click on the image to save it to your computer." title="Right click on the image to save it to your computer.">

<br><br><br>
<img src="https://lavaboxdeclarativescheduler-dev-ed--c.ap4.content.force.com/servlet/servlet.ImageServer?id=0156F00000Cf6LD&amp;oid=00D6F000000EMro&amp;lastMod=1482131682000" alt="Right click on the image to save it to your computer." title="Right click on the image to save it to your computer.">



<br>
# Version 0.1
<a href="https://githubsfdeploy.herokuapp.com/app/githubdeploy/dthowell/DeclarativeScheduler">
<img  class="alignnone size-full wp-image-1966" src="https://andrewfawcett.files.wordpress.com/2014/09/deploy.png?w=820" alt="deploy">
</a>
And a quick managed package link:
https://login.salesforce.com/packaging/installPackage.apexp?p0=04t6F000000Bt1N



<br><br><br>
# Credit:
Douglas for showing me the idea and for some of his code :) https://github.com/DouglasCAyers/sfdc-add-contacts-to-campaign-report-service
<br><br>
Andy For all of his work in the area. And for me to learn off soem of his code https://andyinthecloud.com/2016/02/28/dynamically-creating-flows-in-apex/


