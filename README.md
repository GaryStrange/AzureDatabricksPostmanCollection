# AzureDatabricksPostmanCollection
Azure Databricks exposes a comprehensive admin and job execution API. This postman collection provides merely a convenient way of interacting with the Databricks API.

If you're coming from a spark background have gotten used to administrating clusters via spark shell, this is a convenient alternative when migrating over to Databricks.

# Environments
The collection expects a couple of environment variables.

*authToken = ???*

You'll need to [generate an authToken](https://docs.azuredatabricks.net/api/latest/authentication.html#generate-a-token), from your Azure Databricks workspace, to interact with the API.

*ClusterId = 0118-131427-cools355*

Some of the requests will require a cluster id, for instance, 'POST Start Cluster'. The easiest way to populate a ClusterId variable is to call the 'GET List Clusters' request and then find the cluster id in the list of clusters returned.

*NotificationEmail = me@domain.com*

Jobs definition can include alert notifications such as Job Start, Job Failed, etc. Populate this variable to send these notifications to an email address of your choosing.

# References
https://docs.azuredatabricks.net/api/index.html
