I run a Icecast stream for the use of myself and my friends, and while making playlists for it, I was very overcome by the enormity of the task. I have a modest OGG collection by some standards, 2500 tracks. I pity anyone that has ever tried to make playlists for a large streaming site with who knows how many tracks. What's more, I can't be bothered to switch playlists out all the time. So the natural progression seemed to be a simple drag-and-drop interface to create and schedule playlists.

I plan to use a separate backend from the web interface, so that a X-based frontend could be added eventually, or support could be added in an existing media application. SQLObject will be used to provide support for multiple databases with one set of code. I will try to minimize configuration to media path, and database connections, and password for the interface.

I have some code written, a script that populates a database, and a script that will be called by Ices and Icecast that provides the next track to play. I wish to include searching/adding media to a playlist based on metadata, as the populate.py script parses OGG tags and adds them to the database.

The frontend will be based off of TurboGears (http://www.turbogears.org) and could be packaged as a python egg, separately or included with the source for the backend. In the event that no playlist is scheduled, there will be a random playlist that will be automatically generated. Future plans are to integrate with Google Calendar, to display to any users which playlists will be scheduled. Another of my plans is to research integration with Icecast, to add support for controlling it. I've been thinking about this project and planning it since December, and I am extremely excited.

The main focus of this project is ease, and I will facilitate use in these ways:

1. Simple Interface, very self-explanatory.
2. Minimal configuration. No web server needed, no PHP, extremely easy to get up and running. (Possibly) a few Python Libraries to install. One short configuration file. However, Ices will need to be configured to accept input from a script.
3. Database agnostic. If no database server is installed, SQLite will work perfectly in it's stead.

My goals in this project are not overly ambitious, and will contribute greatly to media enthusiasts like myself. I have set up a project page on Google Code (http://code.google.com/p/icebreaker/). I have not released any code because the code is not usable by anyone other than myself for the initial development. Soon I will add the code I have completed to the project page after adding database support to the Ices-callable script. I realize this description is very short in comparison to the 7500 character limit, but a few details are currently "up in the air". Namely, how I will handle scheduling and whether or not I will daemonize the backend. I have several ideas on how to handle the internals, but it's too early to tell how it will work. Very soon I plan on doing a few flowcharts to illustrate the architecture of the project, and the various ways it may manifest.

I plan on having this application feature complete about 75% through the summer, as I am already greatly obsessed with it and am only abstaining from the project to focus on my schoolwork. I have the entire summer to work on this project if it is accepted and will spend at least 30 hours a week on it. Almost everything I code is media-oriented. I usually write converter scripts in python or bash to manipulate files. I am most comfortable in Python and I have done a little work in C. I also took a course in VB.net and hated every minute of it. I dont think of myself as a programmer, but I greatly enjoy making things and enjoying the outcome of my labor.

My name is Nicholas Mudd and I am currently a student at Illinois Central College in Peoria, Illinois majoring
in Microcomputer Network Administration (they shortened this to 'Network Specialist' at the start of this last semester but I like the old program name better). My email address is nickmudd@gmail.com and my nick on Freenode is nickmudd.

Though I wont contribute specifically to any one of your projects in code, I feel that my project will enhance other xiph projects.

