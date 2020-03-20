# User Authenticated Chat Room Browser App: (TypeScript + Node.js + SQL)


***


## A locally hosted http REST API, made in Typescript and Node, with Express and Socket.IO frameworks, supported by a MySQL database.

### <i> Login/Register and join the chatroom, presented in real-time and dynamically. Manage your account, such as changing password or username (which are both needed to login!). Account information is all queried/edited/stored via a MySQL database.

<br>

***

### Client Page (Front-End) Homepage: <br>
#### <b>http://localhost:<Port\>/</b>

***

<br>

***
***

<br>

|Version| Changes|
|:---|:---|
|Version 0.0.1 [2020-03-08]|<ul><li>Initial Commit.</li><li>Add inital directory structure and files.</li><li>Build enables users to join, set a name (or not) and chat with each other.</li><li>Add dynamic 'who is typing' live indicator</li><li>Set un-changable unique ID to users, to trace all messages back to users.</li><li>Add logging/informative details about who connects/disconnects.</li><li>Add timestamp and further styling to messages.</li><li>Add Screenshots dir, and image screenshot files.</li><li>Add README.md</li></ul>|
|Version 0.0.2 [2020-03-09]|<ul><li>Add new set to store chat/conversation history, which is sent to newly connected clients (enables full chat when client joins later/last).</li><li>Remove 'dist' and 'modules' folders. (After adding gitignore.)</li><li>Update README.md</li></ul>|
|Version 0.1.0 [2020-03-10]|<ul><li>Add connected users list to client-side.</li><li>Add new IUser type for user's details, and create new set to hold these (and ammend IMessage type to accept this new type in place of exisiting props).</li><li>Update front-end DOM and appearance, to be more sensical.</li><li>Update public script to accept newly updated types/interfaces.</li><li>Update README.md</li></ul>|
|Version 0.2.0 [2020-03-11]|<ul><li>Update connected users list on client-side, plus styling.</li><li>Update chatroom/message-list to have a scroll (overscroll) feature, for large amounts of messages.</li><li>Add feature to always scroll to bottom of chatroom/messages-list.</li><li>Update the user set list to remove contacts on disconnection, and send updated list out to remaining.</li><li>General code sharpening.</li><li>Update 'Screenshots' dir, with new images.</li><li>Update README.md</li></ul>|
|Version 0.2.1 [2020-03-12]|<ul><li>Add feature to show all users who may be typing concurrently (so more than one at a time).</li><li>Add server messages feature, to alert connected users of updates to other connected users. I.e. connecting/disconnecting.</li><li>Fix bug, where when any user sends a message it would clear all user's input field of text.</li><li>General code sharpening/tidying, and minor client-side DOM adjustments.</li><li>Update README.md</li></ul>|
|Version 0.2.2 [2020-03-13]|<ul><li>Friday the 13th Update, spoooky.</li><li>Add basic mySQL database infrastructure and connection.</li><li>Update Screenshots.</li><li>Update README.md</li></ul>|
|Version 0.2.3 [2020-03-17]|<ul><li>Add further mySQL database infrastructure, including add a new entry row comprised of ID(Pri Key), Username and Password(Hashed).</li><li>Add new front-end form, for use to make a post request on register button, to add new user details to db.</li><li>Add new dependacy/module, for parseing request body.</li><li>Update README.md</li></ul>|
|Version 0.3.0 [2020-03-20]|<ul><li>Big Update - Full SQL Database Integration and Support.</li><li>Add full user authentification to login client page, in order to access chatroom.</li><li>Complete the login client page registration feature, including adding new users as a row to sql db.</li><li>Full chatroom username and unique ID integration with sql db - all details are pulled from db.</li><li>Add my account section to chatroom client page, with an account overview.</li><li>Ability to change password in the my account section of chatroom, reflected into db also.</li><li>Update change username to also update account section and sql database entry.</li><li>Redirections: When not logged in, always redirect too the login client page. When logged in, always redirect to chatroom client page.</li><li>Update README.md</li></ul>|