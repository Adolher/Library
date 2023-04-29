# User Document

```mongoDB
{
  user: "<name>",
  pwd: passwordPrompt(),      // Or  "<cleartext password>"
  customData: { <any information> },
  roles: [
    { role: "<role>", db: "<database>" } | "<role>",
    ...
  ],
  authenticationRestrictions: [
     {
       clientSource: ["<IP>" | "<CIDR range>", ...],
       serverAddress: ["<IP>" | "<CIDR range>", ...]
     },
     ...
  ],
  mechanisms: [ "<SCRAM-SHA-1|SCRAM-SHA-256>", ... ],
  passwordDigestor: "<server|client>"
}
```

| key | value | description |
| --- | --- | --- |
| user | *string* | name of the user |
| pwd | *string* or `passwordPromt()`| the users password |
| customData | *document* | (optional) custom Data |
| roles | *array* | roles granted to the user; empty array -> user without roles |
| authenticationRestrictions | *array* | (optional) specifies a list of IP addresses and CIDR ranges from which the user is allowed to connect |
| mechanisms | *array* | (optional) specify the SCRAM mechanism or mechanisms for creating SCRAM user credentials |
| passwordDigestor | *string* | (optional) indicates whether the server or the client digests the password |
