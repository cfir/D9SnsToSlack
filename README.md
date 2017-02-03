# D9SnsToSlack
Lambda function for pushing events from SNS to Slack

Modified from the Cloudwatch to Slack template and adopted for Dome9  1.19.2017

Variables needed:
hookUrl - slack webhook url
slackChannel - individual channel to post to

Optional variable:
messageTypeBlacklist - pipe delimited list of message types to NOT post to slack. This is to help reduce noise

The top 3 most common events you might want to filter are:
InstanceStateChanged
InstanceCreatedEvent
InstanceTagsChangeDetectedEvent
