# SERVISKO 
It is a purpose-built platform designed to connect service seekers and service providers specifically within the University of the Philippines Visayas (UPV) community. The platform aims to centralize service discovery, coordination, and communication, replacing the traditional reliance on manual referrals and scattered social media posts.  
### Core Features
- *Role-Based Access*: Users can sign up as a service seeker (finding people to perform tasks) or a service provider (applying to tasks). The system also allows a single user to hold both roles simultaneously. Authentication is restricted to UP mail accounts.
- *Service Listings & Discovery*: Service seekers have full control to create, edit, delete, and archive listings. Users can browse, search, and filter through these listings or search for specific service provider profiles.
- *In-Platform Messaging*: The app includes a real-time chat system. Seekers can message providers directly from their profiles , and providers can communicate with seekers for any listings they have applied to.
- *Application Tracking*: The platform provides progress monitoring for both parties. Providers can track if their application status is pending, accepted, or rejected , while seekers can manage all applications received for their specific listings.
- *Safety and Administration*: Users can report suspicious listings or providers to maintain community standards. A dedicated Admin role exists to monitor platform statistics and resolve reported issues.

## Requirements-Based Testing 
  ### REQUIREMENT #1

| Field             | Value                                                                                                         |
|-------------------|---------------------------------------------------------------------------------------------------------------|
| Requirement       | "The admin is able to view the platform statistics (i.e. how many users there are, how many listings, etc.)"  |
| Test Input/Action | Logged in using the admin credentials and navigated to the Admin Dashboard to observe the displayed platform statistics and dashboard functionality. |
| Expected Result   | The dashboard should correctly display platform statistics such as total users, listings, reports, and pending reports without significant loading delays or interface issues. |
| Actual Result     | The admin dashboard successfully displayed the platform statistics including total users, listings, reports, and pending reports. However, the dashboard statistics took noticeable time to load after refreshing the page. Additionally, the icons used for the statistics cards appeared similar to clickable buttons, which may confuse users regarding their functionality. Despite these usability concerns, the dashboard functioned properly overall. |
| Pass / Fail       | ✅ Pass |   

  ### REQUIREMENT #2

| Field             | Value                                                                                                         |
|-------------------|---------------------------------------------------------------------------------------------------------------|
| Requirement       |“Users are able to sign in using UP mail”   |
| Test Input/Action | Sign in using my up mail. |
| Expected Result   | Successfully logged in using my UP Mail |
| Actual Result     | Was not logged in. The button for logging in with UP Mail was not working.  |
| Pass / Fail       | Fail ❌ |   

### REQUIREMENT #3

| Field             | Value                                                                                                         |
|-------------------|---------------------------------------------------------------------------------------------------------------|
| Requirement       | “Service seekers are able to create, edit, and delete listings.”  |
| Test Input/Action | Added a new listing with a title “Tutor for Math 54” and search and filter listings |
| Expected Result   |Listing is created and shown in the Listings page, and can be edited and deleted while also being able to search and filter from the listings provided. |
| Actual Result     | The listing was created successfully with a toast confirming it but does not reflect in the Listings page. Successfully searched and filtered listings. However, the listing is only reflected in the User’s My Listings page and can be edited but shows an error message when deleting it. |
| Pass / Fail       | Fail ❌ |   

 ### REQUIREMENT #4

| Field             | Value                                                                                                         |
|-------------------|---------------------------------------------------------------------------------------------------------------|
| Requirement       |“Service providers are able to apply to listings.”   |
| Test Input/Action | Apply to a listing entitled “Mobile App Debugging” and search and filter listings to apply |
| Expected Result   | Application is successful and is shown in the My Applications page with a pending phase and successfully searched and filtered from the listings provided. |
| Actual Result     | The application for the listing is successful and is shown in the My Application page as a pending status. Search and filter was successful from the listings provided. |
| Pass / Fail       | Pass ✅ | 

 ### REQUIREMENT #5

| Field             | Value                                                                                                         |
|-------------------|---------------------------------------------------------------------------------------------------------------|
| Requirement       |“Users are able to view service provider profiles.”   |
| Test Input/Action | Pressed on the “Find Providers” button.  |
| Expected Result   | A list of service provider profiles is displayed. |
| Actual Result     | Successfully displayed all service provider profiles, with additional features including search, filtering, and sorting options (e.g., by newest or listing view).  |
| Pass / Fail       | Pass ✅ | 

 ## REQUIREMENT #6

| Field             | Value                                                                                                         |
|-------------------|---------------------------------------------------------------------------------------------------------------|
| Requirement       |“Users are able to search and filter service providers. ”   |
| Test Input/Action |Entered “tutoring” in the search bar and selected “Tutoring” from the skills filter.  |
| Expected Result   | Only service providers listed under the “Tutoring” category are displayed. |
| Actual Result     |Successfully displayed all tutoring-related service providers. Both search and filtering functioned correctly, with results updating in real time.  |
| Pass / Fail       | Pass ✅ | 

 ### REQUIREMENT #7

| Field             | Value                                                                                                         |
|-------------------|---------------------------------------------------------------------------------------------------------------|
| Requirement       |“Users are able to chat service providers through their profile and chat with service seekers they have applied to.”   |
| Test Input/Action | Logged in as a Seeker, clicked on Service Providers, selected one of the Providers in the list, clicked message, and sent messages.  Logged in as a Provider, clicked message, and sent messages.  |
| Expected Result   | Successful delivery of messages from Seeker to Provider and vice versa. |
| Actual Result     | Successfully sends message and displays it with time sent.  |
| Pass / Fail       | Pass ✅ | 

 ### REQUIREMENT #8

| Field             | Value                                                                                                         |
|-------------------|---------------------------------------------------------------------------------------------------------------|
| Requirement       |“Users are able to report listings and/or service providers.”   |
| Test Input/Action | Logged in as a Seeker, went to listings and service providers tab and clicked on flag icon to report listing and a provider.  |
| Expected Result   | Leave a reason and submit it successfully. |
| Actual Result     | Admin received the report and is able to take action in the report list.  |
| Pass / Fail       | Pass ✅ | 

### REQUIREMENT #9

| Field             | Value                                                                                                         |
|-------------------|---------------------------------------------------------------------------------------------------------------|
| Requirement       |“The admin is able to view the platform statistics (i.e. how many users there are, how many listings, etc.).”   |
| Test Input/Action | Logged in using the admin account and accessed the Dashboard page. Refreshed the page multiple times and observed the statistics cards displaying Total Users, Total Listings, Total Reports, and Pending Reports.   |
| Expected Result   | The admin dashboard should correctly display platform statistics in real time. |
| Actual Result     | The dashboard successfully displayed all required statistics including Total Users, Listings, Reports, and Pending Reports. However, after refreshing the page, there was a noticeable delay before the statistics were fully loaded. Additionally, the statistic cards/icons appeared visually similar to clickable buttons even though they were non-interactive, which may confuse users.  |
| Pass / Fail       | Pass ✅ | 

### REQUIREMENT #10

| Field             | Value                                                                                                         |
|-------------------|---------------------------------------------------------------------------------------------------------------|
| Requirement       |“The admin is able to view reports and decide what to do with them.”   |
| Test Input/Action | Logged in as a regular user and submitted reports against a listing/provider. Then logged in as an admin and accessed the Reports page. Tested the available actions including View, Resolve, and Dismiss.  |
| Expected Result   |  The admin should be able to view submitted reports and manage them appropriately through available moderation actions. |
| Actual Result     | Admin can view and decide what to do with reports successfully Reports page. The Resolve and Dismiss actions functioned correctly and updated the report status. However, there are some minor usability issues were observed: The “View” (eye icon) button did not appear to perform any visible action. The trash icon was initially interpreted as a delete function, but it actually marks reports as “Dismissed.” After resolving a report, the Resolve button disappears, while dismissed reports still retain some action buttons, creating inconsistent behavior. The moderation controls may be confusing for first-time users/admins due to unclear icon meanings and inconsistent UI feedback.|
| Pass / Fail       | Pass ✅ | 

# Scenario-Based Testing

  ### Scenario #1: Service Seeker Creates a Tutoring Listing
  
  **User Story:**  
  "As a user, I want to sign up using my UP mail and create a listing for a tutoring service, so that I can find a service provider within the UPV community."
  
  | Step | Action | Expected Behavior | Result | Remarks |
  |---|---|---|---|---|
  | 1 | Open the ServIsko app | The landing/login page should load properly. | ✅ Pass |  |
  | 2 | Attempt to sign up using UP Mail | The user should be able to create an account and be redirected to the platform. | ❌ Fail | The UP Mail sign-in button did not work. |
  | 3 | Create an account manually | The user should be able to access the platform. | ✅ Pass | |
  | 4 | Create a new listing for a tutoring service | The listing should be created and visible to service providers through the Listings page. | ❌ Fail | The listing was created, but it did not reflect on the Listings page. |
  | 5 | Check the “My Listings” page | The listing should appear under the user’s created listings. | ✅ Pass | |
  | 6 | Edit the created service listing | The user should be able to update the listing details. | ✅ Pass | |
  | 7 | Search and filter other tutoring service listings | The system should display listings based on the search/filter input. | ✅ Pass | |

  ### Scenario #2: Service Provider Searches and Applies to a Listing
  
  **User Story:**  
  "As a user, I want to search for service listings and apply to one, so that I can offer my services to a seeker."
  
  | Step | Action | Expected Behavior | Result | Remarks |
  |---|---|---|---|---|
  | 1 | Open the ServIsko app | The landing/login page should load properly. | ✅ Pass |  |
  | 2 | Log in using a service provider account | The user should be able to access the platform as a service provider. | ✅ Pass | |
  | 3 | Go to the Listings page | The system should display all available service listings. | ✅ Pass | |
  | 4 | Search and filter listings | The system should display listings based on the search/filter input. | ✅ Pass | |
  | 5 | Select and apply for the listing titled “Mobile App Debugging” | The system should display the details of the selected listing, and the application should be submitted successfully. | ✅ Pass | |
  | 6 | Go to the “My Applications” page | The submitted application should appear in the user’s applications list with a "Pending" status. | ✅ Pass | |

  ### Scenario #3: Admin Reviews Platform Statistics and Manages Reports

  **User Story:**
  "As an admin, I want to view the platform statistics and manage submitted reports, so that I can monitor the platform and take action on reported listings or users."

   | Step | Action | Expected Behavior | Result | Remarks |
  |---|---|---|---|---|
  | 1 | Open the ServIsko app | The landing/login page should load properly. | ✅ Pass |  |
  | 2 | Log in using an admin account | The admin should be redirected to the admin dashboard. | ✅ Pass | |
  | 3 | View and analyze platform statistics | The dashboard should display platform statistics, including Total Users, Total Listings, Total Reports, and Pending Reports. | ✅ Pass | |
  | 4 | Go to the "Reports" page | The system should display the submitted reports. | ✅ Pass | |
  | 5 | Go through the reports' details |The system should show more details about the selected report when the "View" or eye icon is clicked. | ❌ Fail | The View button did not show any visible action. |
  | 6 | Resolve a report | The selected report should be marked as resolved, and the report status/actions should update properly. | ✅ Pass | |
  | 7 | Dismiss a report | The selected report should be marked as dismissed. | ✅ Pass | |
  

  



