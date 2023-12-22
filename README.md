# Grindery Status

This repository contains a single JSON file that represents the status of various services of the Grindery network.

The status of each service is represented as either "on" or "off" (boolean true/false).

Additionally the file contains status of various activities available for the user.

## File Structure

The JSON file has a simple structure. There are two main groups: `services` and `activity`. Each key in the group is name of a service and the value is the status of the service.

```json
{
  "services": {
    "bot_api": true // change to `false` to indicate that service is down
  },
  "activity": {
    "send": true // change to `false` to disable tokens sending
  }
}
```

## Usage

This file will serves as a data source for a page that indicates the status of the Grindery network and related services. The file is publicly available and can be accessed directly from the repository: https://raw.githubusercontent.com/grindery-io/grindery-status/main/status.json.

## Updates

The file is updated manually by the repository owner.

## Contributing

As this repository is manually maintained by the owner, contributions are not required. However, if you notice any discrepancies in the service status, please raise an issue.
