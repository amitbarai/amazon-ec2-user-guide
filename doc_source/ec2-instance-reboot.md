# Reboot Your Instance<a name="ec2-instance-reboot"></a>

An instance reboot is equivalent to an operating system reboot\. In most cases, it takes only a few minutes to reboot your instance\. When you reboot an instance, it remains on the same physical host, so your instance keeps its public DNS name \(IPv4\), private IPv4 address, IPv6 address \(if applicable\), and any data on its instance store volumes\.

Rebooting an instance doesn't start a new instance billing period \(with a minimum one\-minute charge\), unlike stopping and restarting your instance\.

We might schedule your instance for a reboot for necessary maintenance, such as to apply updates that require a reboot\. No action is required on your part; we recommend that you wait for the reboot to occur within its scheduled window\. For more information, see [Scheduled Events for Your Instances](monitoring-instances-status-check_sched.md)\.

We recommend that you use the Amazon EC2 console, a command line tool, or the Amazon EC2 API to reboot your instance instead of running the operating system reboot command from your instance\. If you use the Amazon EC2 console, a command line tool, or the Amazon EC2 API to reboot your instance, we perform a hard reboot if the instance does not cleanly shut down within four minutes\. If you use AWS CloudTrail, then using Amazon EC2 to reboot your instance also creates an API record of when your instance was rebooted\.

**To reboot an instance using the console**

1. Open the Amazon EC2 console\.

1. In the navigation pane, choose **Instances**\.

1. Select the instance and choose **Actions**, **Instance State**, **Reboot**\.

1. Choose **Yes, Reboot** when prompted for confirmation\.

**To reboot an instance using the command line**

You can use one of the following commands\. For more information about these command line interfaces, see [Accessing Amazon EC2](concepts.md#access-ec2)\.
+ [reboot\-instances](https://docs.aws.amazon.com/cli/latest/reference/ec2/reboot-instances.html) \(AWS CLI\)
+ [Restart\-EC2Instance](https://docs.aws.amazon.com/powershell/latest/reference/items/Restart-EC2Instance.html) \(AWS Tools for Windows PowerShell\)