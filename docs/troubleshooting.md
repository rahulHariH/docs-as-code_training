# Troubleshooting

This topic provides information about troublesshooting issues that you might encounter when using the product.

<details>
<summary>Jira fails to authorize you when BMC Defender Server attempts to create a Jira issue from an action</summary>
 
If Jira returns an authorization error when BMC Defender Server attempts to create a Jira issue from an action, perform the following actions to resolve the issue:

- Make sure that there are no trailing spaces in the API token value.
- Verify that the Jira user email and API token are correct.
- Confirm that the Jira user has permission to create issues in the target project.
 
</details>

<details>
<summary>Jira issue created from an action doesn't display information based on your updates to the script file</summary>
 
If a Jira issue created by a BMC Defender Server action doesn't display the right information based on your updates to the **JiraITSM.bat** (or your custom script) file, perform the following actions in sequence:

1. Delete the existing **JiraITSM.bat** file from the **_installationDirectory_\t-actions** directory.
1. Replace **_installationDirectory_** with the directory in which you installed the product. The default directory is **C:\Program Files\BMC Software\BMC Defender**.
1. Install the latest version of the product or apply the latest PTF.
For more information, see [Installing](installation.md) or [Upgrading](administration.md).
1. Update **JiraITSM.bat** with your custom values or create your custom script.
For more information, see [Configuring a ticket action to create Jira issues](getting-started.md).
1. Update the action on the Actions tab with the updated script.
For more information, see [Creating, editing, and testing ticket actions](troubleshooting.md).
 
</details>

## Where to go from here

For more information about installing the product, see [Installing BMC Defender Server](installation.md).