---

copyright:
  years: 2016,2018
lastupdated: "2018-05-07"

keywords: postgresql, compose

subcollection: ComposeForPostgreSQL

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}

# Connecting an {{site.data.keyword.cloud_notm}} application
{: #ibmcloud-cf-app}

To connect an {{site.data.keyword.cloud}} application to your service, use the service credentials that are created when the service is provisioned.

## Connecting using the 'Hello World' sample app

The [sample app](https://github.com/IBM-Bluemix/compose-postgresql-helloworld-nodejs) demonstrates how to use Node.js to connect to a {{site.data.keyword.composeForPostgreSQL}} service by using the provided credentials. The application creates, reads from, and writes to a database.

Download the sample app and follow the instructions in the readme file. Then, in your application details page in {{site.data.keyword.cloud_notm}}, click **View APP** to view the contents of the *examples* table.

## Available credentials

Field Name|Description
----------|-----------
`uri`|The URI to be used when connecting to the service. The URI includes the schema (`postgres:`), admin user name and password, host name of server, port number to connect to, database name and "?ssl=true" to enable SSL connections.
`uri_cli`|A `psql` shell command line that connects to the database instance.
`ca_certificate_base64`|A self-signed certificate that is used to confirm that an application is connecting to the appropriate server. This is base64 encoded. You need to decode the key before using it, as shown in the sample application.
`deployment_id`|An internal identifier for the service as created within Compose.
`db_type`|The type of database that is offered by the service; in this case `postgresql`.
`name`|The database deployment name.
`uri_direct_1`|A secondary URI that can be used when connecting to the service. Formatted as for `uri`.
`uri_cli_1`|A secondary `psql` shell command line that connects to the database instance.
{: caption="Table 1. Compose for PostgreSQL credentials" caption-side="top"}

**Note:** Two `haproxy` portals provide access to the PostgreSQL service. Both `uri` and `uri_direct_1` can be used to connect. In your applications, switch between `uri` and `uri_direct_1` to manage responses to connection failures.