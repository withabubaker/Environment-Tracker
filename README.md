# Tracking Temperature and Humidity using S1 Minew Device, Pareto Anywhere, Node-Red, and MS SQL database

![alt text](https://github.com/withabubaker/Environment-Tracker/blob/main/IMG/dashboard-Screen.jpg)


## Project Goals:

- Using Pareto Anywhere to harness the temperature and humidity data from Minew S1 BLE Sensor.
- Display the data in Node-Red dashboard.
- Store the data in MS SQL database for further analysis.


## Tools & Hardware:

1. Raspberry Pi.
2. [Pareto Anywhere](https://www.reelyactive.com/pareto/anywhere/).
3. [Minew S1 BLE Sensor](https://www.minew.com/product/s1-ble-temperature-and-humidity-sensor/).
4. Node-Red.
5. MS SQL Server Express Edition.


## Installation:

1. Install Pareto Anywhere on Raspberry Pi. Follow the step-by-step instructions available [here](https://reelyactive.github.io/diy/pareto-anywhere-pi/).
   Pareto Anywhere is an IoT middleware that makes extracting data from BLE devices much easier, and it can be installed on local, cloud, and Edge devices.
   ![alt_text](https://github.com/withabubaker/Environment-Tracker/blob/main/IMG/ParetoAnywhereScreen.jpg)
3. Install Node-Red on Raspberry Pi. Step-by-step instructions available [here](https://nodered.org/docs/getting-started/raspberrypi)
4. If required, you can store the data in a database, here I used [MS SQL Server Express edition](https://www.microsoft.com/en-ca/sql-server/sql-server-downloads)
5. Configure Node-Red nodes as required, or import the attached flow.json file. The flow contains these pallets:
     - ***@reelyactive/node-red-pareto-anywhere***: to pull the data from Pareto Anywhere.
     - ***node-red-contrib-mssql-plus***: connect to MS SQL Server.
     - ***node-red-dashboard***: Node-REd Dashboard.

  ![alt text](https://github.com/withabubaker/Environment-Tracker/blob/main/IMG/nodes-screen.jpg)


## Files:
- ***flow.json***: flow nodes.

