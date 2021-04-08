# lwc-flow-example

Example of lwc in a Salesforce screen flow (passing in values, navigation, etc.)

## About

contains:

- minimal flow & flow definition

- example lwc from documentation @ [lightning-flow-support](https://developer.salesforce.com/docs/component-library/bundle/lightning-flow-support/documentation)

![screenshot](https://i.imgur.com/0gGDuqL.png)

## Deploy

Covert with SFDX; This creates a folder called `deploy`

```bash
sfdx force:source:convert -r force-app -d deploy
```

Now you can deploy from the resulting `deploy` directory

```bash
sfdx force:mdapi:deploy -d deploy -w -1  --verbose 
```

📌  Above deploys to the default org set

- Add `-u user@domain.com` or `-u alias` to deploy else where
- To run tests add `-l RunSpecifiedTests -r ApexTestName`

----------------------

Thrown together with 💝 by [Jamie Smith](https://jsmith.dev)
