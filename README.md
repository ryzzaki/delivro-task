## Delivro Task

### Context

Our Delivro accounting team came to you with a request: to help them keep track of invoices related to each shipment. When our clients create shipments, it goes through our carrier partners (FedEx, UPS, GLS, etc.) and we receive invoices for the created shipments from each of these carriers. Our accounting team has no system to keep track of the invoices, and would like to be able to upload the invoice data directly to our system, so that we can match it with the shipments.

However, the carriers will sometimes send incorrect invoices as well! The weight or price could be wrong, in which case our accounting team notices and reports this issue to the carrier. When we receive a corrected invoice it is yet again uploaded for the same Shipment ID / Tracking Number and it is expected that the application will update the shipment with the latest invoice data.

### The Task

Create an application that will contain a page to view all the uploaded data in any way you deem appropriate and an upload preview modal to allow the user to submit the provided JSON data:

- The user wants to upload a JSON file containing the invoices and shipments data (this is provided as `invoices_1.json` to you as part of this task).
- Allow the user to preview the JSON before uploading it to check if there are any mistakes
- Allow the user to submit the data to the backend
- Save the data into a database of your choice on the backend
- The saved data should be retrievable from the database and displayed to the user on the main page

The edge case:

- The user can come back to upload a second JSON file (this is provided as `invoices_2.json`) which contains a mix of some corrected invoices to existing shipments and also new invoices with new shipments. The data structures for `invoices_1.json` and `invoices_2.json` are the same.

### User Stories

- User should be able to upload any of the `invoices_X.json` files
- User should be able to preview the uploaded JSON before submitting it
- User should be able to view uploaded data in the main screen
- User should be able to view the shipments with the latest uploaded invoice price and weight (latest invoice is assumed to be correct)

### Important

- You do NOT have to create an authentication mechanism, the whole process can be public. You do NOT lose any points for not doing this, we do not expect this of you
- You can OPTIONALLY use wireframes found in the `/wireframes` folder for inspiration, but you are strongly encouraged to come up with your own UI/UX
- You can use any database you are familiar with, but we do recommend the usage of relational DBs
- You MUST provide clear instructions on how to install and run the application
- You MUST use any React based framework to create the frontend
- You MUST use TypeScript on the Frontend and the Backend

The **choice of frameworks does not matter** to us besides these conditions.

### Bonus ideas (completely optional)

1. Implement a Docker container to run the app
2. Deploy the application to any infrastructure provider of your choice
3. Implement i18n (English and any other language of your choice)
4. Add payload validation to the backend endpoint using Zod or any other package of your choice

### Final remarks

We do not penalize the usage of AI at all. You can complete this task anyhow you want. With that being said, we do strongly care about the result, and if the project is simply an AI generated slop without any post processing input from your side then your submission will not be a very strong contender. We will follow up with a code review call where you will have an opportunity to explain all of your stack choices and why you have implemented the task in your own way.

### Task Submission

Please push your work to a new PUBLIC repository on your Github or Gitlab profile and share the link to the repository with us. If you have deployed the app anywhere (Vercel, Netlify, etc.) then please share the url link to the deployment with us too.
