# docker compose events

<!---MARKER_GEN_START-->
Receive real time events from containers

### Options

| Name        | Type | Default | Description                               |
|:------------|:-----|:--------|:------------------------------------------|
| `--dry-run` |      |         | Execute command in dry run mode           |
| `--json`    |      |         | Output events as a stream of json objects |


<!---MARKER_GEN_END-->

## Description

Stream container events for every container in the project.

With the `--json` flag, a json object is printed one per line with the format:

```json
{
    "time": "2015-11-20T18:01:03.615550",
    "type": "container",
    "action": "create",
    "id": "213cf7...5fc39a",
    "service": "web",
    "attributes": {
      "name": "application_web_1",
      "image": "alpine:edge"
    }
}
```

The events that can be received using this can be seen [here](https://docs.docker.com/engine/reference/commandline/system_events/#object-types).
