# osticket-examples
Creating example tickets and showing options around day to day workflow at a helpdesk with overlapping permissions across different users.

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

This person did a pretty good job of filling out the support ticket and our systems settings got it to the right team, though, so John doesn't have to edit much. Let's make John write a professional replay to Accountant Maggie that will get the ball rolling on this issue. Click the "Post Reply" icon at the top of the screen or simply scroll down until you reach the text box, and write a reply to Maggie from John.

![7  john's professional reply](https://github.com/user-attachments/assets/651cd38f-9f35-4c48-8b41-3a06c9940c30)
<!-- well done, john -->




