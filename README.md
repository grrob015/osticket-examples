# osticket-examples
Creating example tickets and showing options around day to day workflow at a helpdesk with overlapping permissions across different users.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

In this demonstration I will be showing some examples of tickets that could pop up in day-to-day operations at a business and what that would look like on the helpdesk's side of things. I will be using the osTicket webserver I created in [this demonstration](https://github.com/grrob015/osticket-setup) and the settings I used in [this demonstration](https://github.com/grrob015/osticket-settings), so if you've been following along, log into your Azure virtual machine and open osTicket! (Simply type `localhost/osTicket` into your browswer, as a refresher.)

## Accoutant's Laptop Breaks

Go to your osTicket homepage without logging in and click "Open a new ticket". You should be greeted by a page that looks like this:

![1  new ticket landing page](https://github.com/user-attachments/assets/e08cb1b9-bbbb-4686-8b7a-c8fbc2cd2d74)

For our fake ticket, let's have an accountant's laptop break. It will need to be replaced, but we don't know that yet. Fill in the information like so and then click "Create ticket" to submit it to your helpdesk.

![2  maggie's laptop breaks oh no](https://github.com/user-attachments/assets/c9a1d6c2-061d-41d0-959c-0baa69a22b95)

Since John Doe is on the equipment team and a support agent, let's log in with his credentials and look at the ticket and see what options he has with them. Use the credentials you made for John's account and log in as an agent to your helpdesk.

![3  john sees the ticket](https://github.com/user-attachments/assets/bc80e2b7-3cdf-4c30-b080-0f5871ad46d4)
<!-- astute readers will notice that the ticket isn't exactly the same. Apparently tabbing out of your virtual machine while waiting for osTicket to process causes the ticket to not be created. which like, it's a different machine, why would me not looking at it matter? quantum mechanics? observing things changing the outcome? who knows. -->

Perfect! The ticket has been automatically assigned to the Equipment team and it shows up on John's account. If John clicks on the ticket and decides to work on it, he is presented with numerous options and settings about the ticket that he can change and work with.

![4  john's world of options](https://github.com/user-attachments/assets/aaf3b021-e8b8-43a1-a34e-743bcfe4a7f2)
<!-- it's a whole new worlddddd -->

In the very top row of icons alone, John can: 

![5  dense options](https://github.com/user-attachments/assets/fe2008f0-ea64-469b-8f50-4456ecd97351)

- **Post Reply** - Send a public message to the ticket opener, himself, and anyone else subscribed to the thread of this ticket.
- **Post Internal Note** - Create notes that the end user cannot see about the ticket. This could be things like possible solutions, technical information relating to the ticket, or problems that the end user doesn't need to know about.
- **Change Status** - Marking a ticket as resolved or closed means that the problem has been solved and no more work needs to be done.
- **Print** - Print the entire thread or only certain parts of it if there's something he needs to show someone in real life, possibly a superior or for archival purposes.
- **Edit** - Edit parts of the ticket that the user may not have filled out correctly.
- **More** - Change the owner, Mark as answered, manage referrals, and other miscellaneous tasks involving the ticket.

Just below the title of the ticket, John can edit any of the clickable items and change things like the SLA, help topic of the ticket, and more.

![6  more options for john](https://github.com/user-attachments/assets/4553ac16-0dcd-4cbb-a584-2bb902ddc3a0)

This person did a pretty good job of filling out the support ticket and our system's settings got it to the right team, though, so John doesn't have to edit much. Let's make John write a professional replay to Accountant Maggie that will get the ball rolling on this issue. Click the "Post Reply" icon at the top of the screen or simply scroll down until you reach the text box, and write a reply to Maggie from John.

![7  john's professional reply](https://github.com/user-attachments/assets/651cd38f-9f35-4c48-8b41-3a06c9940c30)
<!-- well done, john -->

💡 If we go back to our open ticket dashboard, we can see that by replying, John has claimed the ticket. (Contrast this with the picture that says the ticket is assigned to "Equipment".)

![8  the ticket is now johns](https://github.com/user-attachments/assets/80e2d6e4-1c41-4c27-a93a-4f6ecfc85245)

John wants to take some internal notes to remind himself about the steps he'll need to take to troubleshoot the problem, so he posts an internal reply that won't notify Maggie about procedure for broken laptops.

![9  johns internal dialogue](https://github.com/user-attachments/assets/fe81a71e-33c3-417f-bc9f-08fbb4123d46)

Once it's 2pm, Maggie takes the laptop to John, and John finds out that a coffee spill is to blame for the troubles, completely frying all of the internals. He gives Maggie a replacement laptop and files the necessary paperwork to document it. The last step is just to close the ticket! John clicks the ticket and updates its status.

![10  john closes the ticket](https://github.com/user-attachments/assets/8def2798-0bea-43fc-b711-538996bf6b83)

Anyone with permissions can now see that the ticket has been closed, when it was closed, and who closed it. To see closed tickets, go to **Tickets -> Closed -> Today** (John doesn't have access to the Admin panel, just the Agent Panel) and you should find this:

![10  john closes the ticket](https://github.com/user-attachments/assets/ea68e5c8-9ca9-4a34-998b-7d2f5aa48677)
<!-- John's first ticket was smooth, but they only get more difficult and important from here on out. --> 

![11  the closed ticket](https://github.com/user-attachments/assets/4b162f60-98c1-4133-863a-2c70bdcb5079)

## Engineer Notices the Printer isn't Working

Go to your osTicket homepage without logging in and click "Open a new ticket". For our next fake ticket, let's have one of our engineers notice that the printer on his floor isn't working. Let's also say that he's in a rush and didn't select the right help topic for the situation. Something like this should do nicely:

![12  conagher notices the printer is down](https://github.com/user-attachments/assets/1fb3dcb5-16a9-4053-81b3-f7d12be09360)

Let's log in as Jane this time. Go to the agent login page and put in Jane's credentials. You should land on a page that looks like this:

![13  janes landing page](https://github.com/user-attachments/assets/47dd932e-b1fc-4fb8-a091-3e741d623473)

Unlike John, Jane has access to the Admin Panel, as you can see in the top right of the page. She has much more access and permissions in our helpdesk as an Omniadmin/supervisor. She notices the new ticket, clicks on it, and knows that a big meeting for a potential very large client is happening soon, and that the printer could sabotage the whole thing. She changes many things about the ticket properties:

- Changing the priority from "Normal" to "High"
- Assigning the ticket to John
- Changing the SLA plan from "Default SLA" to "High priority"
- Changing the help topic from "General Inquiry" to "Equipment Issues / Communal Equipment Breakage"

She will also post an internal reply that lets John know that this is his new priority and that if he needs help, don't be afraid to ask. 💡 **osTicket keeps track of all these changes to a ticket**, and the ticket thread will look something like this:

![14  janes paper trail](https://github.com/user-attachments/assets/90a84af1-4fd5-49d0-b22f-1d60005e1636)



