## VoteCap - A simple REDCap External Module for Q&A sessions

### What is VoteCap?
VoteCap is a REDCap External Module that allows anonymous participants to ask questions and upvote the questions of others. It is built using Bootstrap for its UI, and uses a single REDCap project for its data storage. It requires REDCap 7.0.0 and later.

### Installation
1. Take the files and folders, and place them in the /redcap/modules/votecap_v1.0/ directory on your REDCap web server.
2. As a REDCap administrator, go to the External Modules page in the Control Center, and enable VoteCap.
3. Use the VoteCap_Project.xml file to create a new REDCap project (go to the +New Project page and select the "Upload a REDCap project XML file" option). 
4. Go to the External Modules page within the new project, and enable VoteCap for the project, in which a new link will appear on the left-hand menu. 

### Usage
1. To add a new Q&A session so that it shows up in the session list in the plugin, simply navigate to the REDCap project you created, and add a new record for each session (one record = one session of questions). The only thing required is to give the record a session name on the Session Info instrument (that's it!). Optionally, you may give it an expiration time if you want the session to disappear from the list at a desired time.
2. Click the VoteCap menu link to view the session list you have created. You may disseminate that page's URL to your participant's, or create a short URL for it or for each of the sessions (e.g., via tinyurl.com).
3. Partipants will then be able to access each session (there is no login required), ask a question, and up-vote any question on any session. If you wish to create a new set of sessions (e.g., for a new event), you may start this process over again by creating a new REDCap project from the XML file, and pointing a bookmark to the plugin.
4. If there is an official answer to a question in a session, a user with access to the REDCap project can navigate to that session's record, open the Session Questions instrument, pulling up that question in the Instance list, and add an answer in the Answer text box, after which that answer will be displayed below that question on the plugin's questions page.