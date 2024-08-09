<p align="center"><a href="#readme"><img src=".github/images/card.svg"/></a></p>

<br/>

Action for sending notifications to [Pachca](https://www.pachca.com) messenger. This action sends basic information provided by the user and information about the event based on the type of event.

### Usage

Add next job into your workflow:

```yml
- name: Send notification to Pachca
  uses: essentialkaos/pachca-action@v1
  with:
    webhook: "https://api.pachca.com/webhooks/XXXXXXXXXXXXXXXXXXXXXXXXXX"
    title: "PR created"
    message: "New PR created in repository"
    type: "new-pr"
```

### Inputs

| Option | Description | Value |
|--------|-------------|-------|
| `webhook`  | Pachca webhook URL | _URL_ |
| `title`    | Notification title | _Title_ |
| `message`  | Notification message | _Message_ |
| `type`     | Notification type | _Type_ |
| `timezone` | Timezone name for formatting dates | `UTC` (_Default_) |

### Outputs

| Option | Description |
|--------|-------------|
| `status-code` | API status code |

### License

[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)

<p align="center"><a href="https://essentialkaos.com"><img src="https://gh.kaos.st/ekgh.svg"/></a></p>
