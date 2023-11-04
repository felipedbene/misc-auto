# misc-auto
Share A Automation Doc with the whole org.

`ShareDocOrgAutomation.yaml` is the main automation file, ready to be copy and pasted and run in to ssm

# Shortcut command 
## CLi command to trigger
`aws ssm start-automation-execution --document-name "ShareDocumentToOrg" --document-version "\$DEFAULT" --parameters '{"AutomationAssumeRole":["arn:aws:iam::249477202910:role/test-share-doc"]}' --region us-east-1`

Automation role minimum permission is `required-permison.json` as well as the role trust `trust-policy.json`

## Web Cli
`https://us-east-1.console.aws.amazon.com/systems-manager/automation/execute/ShareDocumentToOrg?region=us-east-1#AutomationAssumeRole=arn%3Aaws%3Aiam%3A%3A249477202910%3Arole%2Ftest-share-doc`
