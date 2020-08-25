---
description: >-
  Follow these steps to connect to your Amazon Web Services (AWS) Relational
  Database Service (RDS) database using WayScript.
---

# Connecting to AWS RDS

## Configuring Your Database

### Enable Public Accessibility

To connect to your database using WayScript, your database must be publicly accessible. Enable "Public accessibility"  in the settings for your database.

![Enabling public accessibility in RDS settings](../../../.gitbook/assets/screen-shot-2020-08-22-at-10.56.35-am.png)

### Update your Security Group Settings

You will also need to update the settings for the security group associated with your DB instance. Configure the "Inbound rules" for the security group to allow all public connections to the port your database communicates on, or whitelist the specific IP addresses used by WayScript.

![Configure your security group to allow public access to the port your database communicates on](../../../.gitbook/assets/screen-shot-2020-08-22-at-10.54.12-am.png)

💡 You can find the current list of WayScript's IP Addresses in the page below:

{% page-ref page="../../../other-information/ip-addresses.md" %}

💡 You can find the security group associated with your DB instance by checking the "Connectivity & Security" tab for your database instance in the AWS console.

![Check these settings from the &quot;Connectivity &amp; Security&quot; tab for your database instance](../../../.gitbook/assets/screen-shot-2020-08-24-at-5.15.38-pm.png)

### Additional References

* [How can I troubleshoot connectivity to an Amazon RDS instance that uses a public or private subnet of a VPC?](https://aws.amazon.com/premiumsupport/knowledge-center/rds-connectivity-instance-subnet-vpc/)
* [A DB Instance in a VPC Accessed by a Client Application Through the Internet](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_VPC.Scenarios.html#USER_VPC.Scenario4)

## Obtaining Connection Information

To connect to your database using WayScript, you will need the following information:

![Information required for WayScript to connect to a database hosted in AWS RDS](../../../.gitbook/assets/screen-shot-2020-08-22-at-11.03.30-am.png)

### Endpoint & Port

The Endpoint and Port information is available in the "Connectivity & Security" tab for the database instance in the AWS console.

![Endpoint &amp; port settings for database instance in AWS console](../../../.gitbook/assets/screen-shot-2020-08-24-at-5.13.41-pm.png)

### Database Name

The Database Name is available in the "Configuration" tab for the database instance in the AWS console.

![DB name, as displayed in the AWS Console](../../../.gitbook/assets/screen-shot-2020-08-24-at-5.21.12-pm.png)

{% hint style="warning" %}
DB name is _**NOT**_ the same as DB instance id
{% endhint %}

💡 If your "DB name" field is blank, this is probably because you did not specify a database name when creating the database instance, under "Additional configuration."

![Setting the Initial database name](../../../.gitbook/assets/screen_shot_2020-08-22_at_11.59.45_am.png)

### Master Username \(User\)

The Master Username is available in the "Configuration" tab for the database instance in the AWS console, under the "Availability" section.

![Master username setting under &quot;Availability&quot; settings for DB instance](../../../.gitbook/assets/screen-shot-2020-08-22-at-11.04.01-am.png)

### Master Password \(Password\)

The Master Password was set when you created your DB instance. If you forgot this password, you can "Modify" your database instance and change the password.

![Setting a new master password for your DB instance](../../../.gitbook/assets/screen-shot-2020-08-24-at-5.28.14-pm.png)

