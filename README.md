# md_policealert
Job based alert system for RedM servers using the VORP Core framework
 
 # About
 MDPA You can use this script to send an alert out to everyone with a specific job title i.e. `police`. If you are interested in what is to come for this script then check out *To Do* to see everything I have planned for it!
 
 # Installation
 - Place `MD_policealert` in your `resources` folder
 - Add `ensure MD_policealert` to your `server.cfg`
 
 # Usage
 - Using this resource is fairly simple. Just place this line where ever you need the police to be alerted
 ```lua
 TriggerClientEvent('md:alert', source, message, time, jobname) -- For server files
 TriggerEvent('md:alert', message, time, jobname) -- For client files
 ```
 - Some obvious things: `message` needs to be a string and `time` how long you want the alert to be visible in seconds(the second to millisecond conversion is baked into the script) and `jobname` should be a string of the job name as it shows up in the database i.e. `'police'`
 - Heres a full example for client and server triggers
 ```lua
 TriggerClientEvent('md:alert', source, 'Robbery at Valentine General Store!', 5, 'police') -- For server files
 TriggerEvent('md:alert', 'Robbery at Valentine General Store!', 5, 'police') -- For client files
 ```
 
 # To Do
- Add other identifiers to send the alert to(not sure what identifiers to use yet but we'll see)

# Notes
- If anybody has any suggestions feel free to open up an issue ticket and if it's something I can do then I'll probably do it if i feel like it lol
- Please keep in mind that I made this thing while on like 2 hours of sleep and being awake for about 16 hours so i was MAD tired lol. if there any issues or things that could have been done better please either open up an issue or make a pull request.
- I do plan on making this resource better but for now it works as intended so until i have the time/energy to work on it this thing is probably just gonna stay the way it is lol


#ONLEY FOR REDM VORP

