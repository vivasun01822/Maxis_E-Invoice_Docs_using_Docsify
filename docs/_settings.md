# Settings

The Settings section offers various configuration options to customize and manage the application. It allows you to adjust essential parameters and preferences to optimize the application's functionality according to requirements.

![Settings](../_media/settings/settings1.png)



The Settings section is divided into several sections. They are:


### Users

The Users section provides a comprehensive list of users, displaying their current roles and other essential details, such as Name, Email, Phone, Company, and Status.

To manage users, click the `Action` button, which offers two dropdown options:

1. **Assign Role:** Use this option to assign a new role to a specific user.
2. **Delete User:** Select this option to remove a user from the system.
Please note, only administrators have access to the Settings section.

![Users](../_media/settings/settings12.png)



### Digital Certificate Update

The Digital Certificate Update section displays a list of uploaded digital certificates. Digital certificates are essential in e-invoicing as they authenticate the sender's identity, ensure the invoice's integrity, and comply with legal standards. They verify that the invoice originates from a trusted source and has not been altered during transmission. Additionally, digital certificates fulfill regulatory requirements for secure electronic transactions.

![Digital Certificate](../_media/settings/settings3.png)



To add a new digital certificate, click the `Add Certificate` button. This will open a modal where you can select a digital certificate file from your local storage. Once selected, click the Submit button to upload the certificate.

![Digital Certificate Create](../_media/settings/settings4.png)



### BQ Table Map

The BQ Table Map feature enables automatic submission of e-invoices directly from a BigQuery table. It streamlines the process by triggering submissions automatically whenever new invoices are added to the specified table.

![BQ Table Map](../_media/settings/settings5.png)


To enable auto-submission triggers, add the table to the BQ Table Map by clicking the Add Table button. This will prompt you to input the required details, including the `Server ID`, `Table ID`, `Partition Size`, and `Request Size`. Once you've filled out the fields, click the Create button. Within an hour, the auto-submission process will begin, automatically submitting e-invoices from the specified table.

![BQ Table Map Create](../_media/settings/settings7.png)


### Audit Logs

The Audit Logs feature allows you to monitor and review all application activity. You can easily track actions performed by users within the portal. This feature includes a search option to filter logs by a user's email—simply enter the email and click the `Search` button to view all operations associated with that user. Additionally, a Date Range filter lets you narrow down results to a specific time period. To reset the filters, use the `Reset` button, which clears the fields and retrieves fresh data from the database.

![Audit Logs](../_media/settings/settings10.png)
