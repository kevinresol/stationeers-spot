# Dedicated server for Stationeers hosted on AWS Spot Instances

This is mostly forked from https://github.com/m-chandler/factorio-spot-pricing, plus an API Gateway to start/stop the server via HTTP request. So your friends without your AWS access could start/stop the server too.

API URL can be found in the cloud formation output after the stack is created.

- To check server status: `GET <api-url>`
- To start server: `POST <api-url>?value=Running`
- To stop server: `POST <api-url>?value=Stopped`


