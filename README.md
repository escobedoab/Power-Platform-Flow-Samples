# Power-Platform-Flow-Samples

## Modify permissions in SharePoint with Power Automate
Utilizing the HTTP trigger and SharePoint endpoints, the below cloud flows will automate the removal of a user from the owner's group and another flow to add a new user and remove a user from the site collection group. These were created because there was a need for a Canvas App to be the front end and Power Automate to be the automation tool. I made the flows separately from the Canvas app because it helped it become more versatile. Feel free to swap the trigger for something more suitable to your needs!

### Remove User From Owners Group Flow Sample
Summary: Removes a user from the SharePoint Owners Group
Technical Description: This flow retrieves the user's profile information, sends an HTTP request to SharePoint to get the user ID, sends another HTTP request to SharePoint to get the ID of the Owners group, and finally removes the user from the Owners group in SharePoint.

### Remove Site Collection Admin
Summary: Adds a new user as a site collection admin and removes a user from the site collection admin
Technical Description: This flow sends an HTTP request to SharePoint to add the new user, get the user ID based on the user's email, and add them to the Site Collection Admin group. The initiator's profile is then used in an HTTP request to remove the user's site collection admin privileges in SharePoint.

