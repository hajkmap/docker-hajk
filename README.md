# docker-hajk
A containerized Hajk solution with everything you need supplied. Just run `docker compose up` and you're good to go.

## Information
- Hajk will start on port 3002. If you wish to run it on another port, change the port mapping in `docker-compose.yml`. 
- All of Hajk's configuration is stored inside the persistent `data` directory. `.env` controls the Backend, while the two JSON-files control Admin and Client UIs. 
- The `data/App_Data` stores all layer configuration. This is the folder that Backend writes to and normally you don't have to edit its contents directly. Instead, you let Admin UI commit the changes via requests to Backend. 

## Quick start
1. `docker compose up`. Add `-d` if you want to run it in production and make Hajk restart on server reboot.
1. Hajk will launch on `localhost:3002`. The Admin UI is accessible on `localhost:3002/admin`. 