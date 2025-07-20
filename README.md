<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket. This tutorial expands upon the previous tutorial, osTicket: Post-Installation Configuration.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Step 1: Creating a Ticket</h2>
<br />
<p>
Our first step is to create a Ticket as an end-user. We'll be creating one as an end-user, "Karen", and the Ticket will be related to the Online Banking system. To create a Ticket, we have to use the End Users URL, which is this link below.
</p>

http://localhost/osTicket 

<p>
The page should look like this.
</p>
<p>
<img width="1890" height="1080" alt="image" src="https://github.com/user-attachments/assets/062b2bba-cc7e-4dfc-aac5-666b646c0e87" />
</p>
<p>
To get started, we're going to click the "Create New Ticket" button and create a Ticket as End User Karen.
</p>
<p>
<img width="891" height="767" alt="image" src="https://github.com/user-attachments/assets/da4e1857-9cc0-4f40-8ecb-ee3f0bf1e9da" />
<img width="933" height="415" alt="image" src="https://github.com/user-attachments/assets/db6b8fa7-b5b0-40bb-92dc-ce0c42594b0f" />
</p>
<p>
Now that the ticket has been created, we're going to log in as Help Desk Agent John and observe the ticket's properties. (SLA, Assignment, Department, Priority.)

To do so, we have to use the other link that was provided in the last tutorial, which is this one.
</p>

http://localhost/osTicket/scp/login.php 

<p>
Once you're there, go ahead and log in as John.
</p>
<p>
<img width="1008" height="454" alt="image" src="https://github.com/user-attachments/assets/792f0a71-0e8f-46fa-ab58-27ea05475f4d" />
</p>
<p>
As you can see above, we're logged in as John, and we can see the newly created Ticket by end-user Karen titled "Online Banking Down". Let's go ahead and click on it to observe its properties.
</p>
<p>
<img width="1004" height="846" alt="image" src="https://github.com/user-attachments/assets/2bd70ad2-9281-4cd8-868c-09c6c1286f80" />
</p>
Here, we can view the full properties, including but not limited to: Status, Priority, Department, who it's assigned to, SLA, etc. Now, we're going to go ahead and change the properties like we would if we were working as Help Desk Agent John. Considering the widespread impact of the online banking portal being down, we'll set the SLA to Sev-A. We'll also set the priority of the ticket to Emergency. And finally, we'll assign it to the Online Banking team to route the ticket to the right team and department.
<p>
<img width="700" height="332" alt="image" src="https://github.com/user-attachments/assets/48ae1f72-a6db-44ea-8c04-2935f7b80569" />
<img width="1192" height="484" alt="image" src="https://github.com/user-attachments/assets/b43b8c42-60ca-4eb8-97a5-b0986f3bdaea" />
<img width="859" height="370" alt="image" src="https://github.com/user-attachments/assets/9602a8e0-52b9-48a6-b743-fd67f87e9a78" />
<img width="979" height="294" alt="image" src="https://github.com/user-attachments/assets/c5880d02-e53e-47c9-bd20-2549b733853d" />
</p>
<p>
Now that the ticket's properties have been updated and assigned to the correct team, we will log in as Help Desk Agent Jane to work the ticket to completion.
</p>
<p>
<img width="918" height="491" alt="image" src="https://github.com/user-attachments/assets/a0601659-b556-48c9-b596-48702548f126" />
<img width="1005" height="193" alt="image" src="https://github.com/user-attachments/assets/a01b9843-326e-4cc8-a85f-5ed8788be5c1" />
</p>
<p>
As Jane, we can assign the ticket to ourselves. This is good practice, as it lets John and other agents know that they can focus on another ticket while Jane works on this one.
</p>
<p>
<img width="723" height="344" alt="image" src="https://github.com/user-attachments/assets/4e76b47c-9498-4b7e-9586-1a732bb37df9" />
</p>
<p>
Even if a complete solution isn't found, it's still good practice (and can be required depending on the company and SLA) to provide the end user with updates like the following.
<p>
<img width="952" height="467" alt="image" src="https://github.com/user-attachments/assets/822ffd41-7ee7-4755-a0a9-6bd444d23ac9" />
</p>
<p>
After a bit of research, Jane was able to find a solution to the issue.
</p>
<p>
<img width="948" height="311" alt="image" src="https://github.com/user-attachments/assets/75e741a7-aec0-4a7b-b1c6-968350c0f58c" />
</p>
<p>
Now that the problem is solved, we can go ahead and click on the "Status: Open" property, and changed the ticket from "Open" to "Resolved".
</p>
<p>
<img width="888" height="224" alt="image" src="https://github.com/user-attachments/assets/5b038fe1-73d3-42c9-971b-e832bfc60497" />
<img width="634" height="224" alt="image" src="https://github.com/user-attachments/assets/a8f9a801-864b-4bb8-a706-df31d90c72c5" />
<img width="990" height="278" alt="image" src="https://github.com/user-attachments/assets/84c32160-a962-487c-960f-2f598efc7e78" />
</p>
<p>
As you can see, now that it's been resolved, the ticket is removed from the list of tickets so agents can focus on other ongoing tickets, or if it's empty, be ready for new incoming ones! As an Admin or agent with a lot of permissions, you can still view previous tickets that have been resolved by going to the Agent Panel and then going to Tickets, and clicking Closed.
</p>
<p>
<img width="994" height="152" alt="image" src="https://github.com/user-attachments/assets/8095b535-751d-46c1-965c-5cee333bd3c3" />
</p>
<br />
<h2>Now, let's do another ticket.</h2>
<p>
As an end user named Ken, we're going to create another ticket. This time, the issue is going to be related to the Use of Adobe Software
</p>
<p>
<img width="871" height="844" alt="image" src="https://github.com/user-attachments/assets/2a0f2a18-4571-4ad5-9a9e-0f9959cd495f" />
<img width="946" height="309" alt="image" src="https://github.com/user-attachments/assets/5b714388-02d4-4224-9d69-f534e7bae0ec" />
</p>
<p>
Now that the ticket has been submitted, we're going to log in as Help Desk Agent John and observe and assign properties as well as resolve the ticket.
</p>
<p>
<img width="980" height="183" alt="image" src="https://github.com/user-attachments/assets/9d392abc-fc74-4639-9f9e-c6e061db2a89" />
<img width="1071" height="857" alt="image" src="https://github.com/user-attachments/assets/7fabe22e-2fff-45ab-970a-92989045c3c5" />
</p>
<p>
With the information currently available on the ticket, John chooses to reach out to Ken via phone call. Ken explains that only 2 people are having difficulty accessing the software. John suggests that Ken has the users try to restart their computers as there were a lot of windows updates yesterday. 

Since this issue isn't as serious as the entire Online Banking System being down, we're going to assign the SLA Sev-C, as well as assign the ticket to the Support Team/John Doe.
</p>
<p>
<img width="996" height="327" alt="image" src="https://github.com/user-attachments/assets/6110b399-4b8d-4a63-9e60-d1e5c3327f69" />
</p>
<p>
In situations like this, where information is received through the phone, it's still important to log the information as an update to the ticket, as well as even create a ticket if you become aware of an issue through phone, text, email, app, through word of mouth, etc.

Ken told John over the phone that he would have them try to restart their computers and call us back after lunch. As such, we update the ticket like the following.

</p>
<p>
<img width="954" height="550" alt="image" src="https://github.com/user-attachments/assets/79ab9026-6fd0-4653-a0c5-3fb44a2dccbc" />
</p>
<p>
After lunch, Ken calls John back to inform him that restarting the computers seems to have fixed the issue. With that information, we update the ticket one more time before closing it, like we did before.
</p>
<p>
<img width="970" height="131" alt="image" src="https://github.com/user-attachments/assets/a7be7418-a3a2-4de1-babf-e40ff7766794" />
<img width="691" height="265" alt="image" src="https://github.com/user-attachments/assets/a3f3a34f-10db-4cf5-8bd9-b1a10d1327ff" />
<img width="967" height="72" alt="image" src="https://github.com/user-attachments/assets/d2ae824b-dcdb-42bc-861f-784b008c52a7" />
</p>
