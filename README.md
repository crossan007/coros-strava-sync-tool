#coros-strava
## A tool to automatically sync coros activities to strava

## Instructions
### Configuration method
1. Enter your coros account and password in /etc/config.yaml
2. Enter your strava clientId and screct in /etc/corosstrata-api.yaml (how to get client and screct[https://developers.strava.com/docs/getting-started/])
3. If you have a callback domain name, please fill in the strava callback domain name by mistake.
3. If you are running on a server with a domain name, please configure the callurl with a domain name in /etc/corosstrata-api.yaml configuration, if you are running locally, please keep localhost in the configuration (the callback path is /strava/ callback)

### manual
1. After the program runs, an address will be output, please visit the address manually for the first time, and then click Authorize
2. After receiving the callback authorization from strava, the program will start to refresh the token regularly, and will automatically obtain the coros data of the previous day every day and upload it automatically.

