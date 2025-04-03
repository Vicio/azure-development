Is one of the sections in the settings menu, it allows the configuration of your application by setting the environment variables themselves before the application container activation in the case of Windows, and by sending the environments as parameters in the case of Linux.

There are two types of environment variables allowed to use in Azure, one is the app settings, which enable, disable or preset a specific configuration on your application; and the other one is connection strings, which tell the application about the parameters required to connect to a specific database.

#### App settings

To configure the app settings there are three things you need: the name of the environment variable, the value, and an option whether this variable will be tied to a specific app slot or it will be available to all of them.

Multiple variables can be set using the JSON format as seen here:

```json
[
  {
    "name": "<key-1>",
    "value": "<value-1>",
    "slotSetting": false
  },
  {
    "name": "<key-2>",
    "value": "<value-2>",
    "slotSetting": false
  },
  ...
]
```

#### Connection strings
Connection strings are added in a similar way, the only difference is the parameters required, which are: 
* name: the environment variable name
* value: the connection string in text format (examples can be seen [here](https://www.connectionstrings.com/))
* type: the type of connection string, which is tied to the database you want to connect to
* slot: which applies in the same manner as in app settings

In the same way, multiple connection strings can be configured using a JSON as seen here:
```json
[
  {
    "name": "name-1",
    "value": "conn-string-1",
    "type": "SQLServer",
    "slotSetting": false
  },
  {
    "name": "name-2",
    "value": "conn-string-2",
    "type": "PostgreSQL",
    "slotSetting": false
  },
  ...
]
```

#### CLI
Environment variables can also be configure using the ```az``` command, here is an example:
```bash
az webapp config appsettings set --resource-group <group-name> --name <app-name> --settings key1=value1 key2=value2
```

