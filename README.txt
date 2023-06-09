this project is based on the client/server architecture.Its a web application that is used as a simple
travelling website.
The website allows the users to lookup several travelling destinations. Users create an account,
add places to their “want-to-go list” and search for travelling destinations.
Components:
• Users Login (Main Page):
Registered users are allowed to log in to their accounts using their stored username and
password. If credentials are correct, the user is redirected to the home page. If an
unregistered user tries to log in an error message is displayed.
• User Registration:
Users are allowed to create an account using a username and a password and the users’
information should be stored in a database using MongoDB. If the user tried to register using an
already taken username or left any of the fields empty, an error message is displayed. After
registration, the user is redirected to the login page and a message appears that the
registration was successful.
• Home Page:
The home page is the first page that should be encountered by the users when they log in to their
accounts. It contains several destination categories (Beaches, Mountains, ...etc.) and a button to
view the user’s “want-to-go list”. When the user clicks on any category, they are redirected
to that category’s page.
• Category Page:
The category page contains all the destinations within this category. When a user clicks on any
destination’s name, they are redirected to that destination’s page.
• Destination Page:
The destination page contains a description for the destination. The page also contains an
embedded link for a video describing the destination which can be streamed by the user. Finally, an
“add to want-to-go list” button is added. The button adds this destination to the user’s
“want-to-go list” in the database. If the destination was already in the user’s list, then 
an error message is displayed and the duplicate destination is not added.
• Want-to-Go List Page:
The want-to-go list page contains the destinations that the user previously added using the “Add to
Want-to-Go List” button. A “View Want-to-Go List” button is added to the home page that
directs the user to their own want-to-go list page.
• Search:
A search bar will be displayed in all pages except for registration and login pages. The search will
be done using destinations names only. The search result is either a “Destination not Found”
message if the destination was not available in the database, or a list of the destinations that contain
the search keyword in their names (ex: searching for “div” should put “Maldives” as one of the
results). The search results  are clickable and they direct you to that specific destination’s
page.
