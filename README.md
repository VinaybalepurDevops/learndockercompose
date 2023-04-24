# learndockercompose

The project has been downloaded using https://github.com/samaronybarros/movies-app
The server runs on port 3000
The UI runs on port 8000
The db is mongodb
Create a folder a db inside your project folder and use that as mongo volume
Update ip in server and client folders
There will be cors issues seen in the ui if deployed using docker compose. If we update the parameter newip in the compose file with the public ip of the ec2 instance, the entire set up will work end to end. 
Also it is good to create a volume for the mongo db, which is not done.
