---
weight: 10
title: Upgrading Cumulocity IoT Edge remotely
layout: redirect
---

You can remotely update your instance of {{< product-c8y-iot >}} Edge using the {{< product-c8y-iot >}}'s firmware update feature. This process requires you to upload a YAML file specifying the {{< product-c8y-iot >}} Edge version to your tenant account. For more information about the firmware feature, see [Managing firmware](/device-management-application/managing-device-data/#managing-firmware).

Update the [sample version file](/files/edge-k8s/c8y-edge-version.yaml) to specify the {{< product-c8y-iot >}} Edge version follow the steps below to upgrade:

1. Log in to your {{< product-c8y-iot >}} tenant account and go to the Device Management application.

2. In the **Firmware repository** page, click **Add firmware** and provide a name for the firmware, add a description and its version (all required).

   ![Firmware list](/images/edge-k8s/edge-k8s-firmware-repository.png)

   Optionally, you can define the device type filter when adding a new firmware. For example, *c8y_EdgeAgent*.

3. Select the **Provide a file path** option to specify an HTTPS URL of a server from where the version file can be downloaded.

   Click **Add firmware**. The firmware object appears in the firmware list.

4. Click **All devices** in the **Devices** menu, select your instance of {{< product-c8y-iot >}} Edge from the device list.

5. Click **Firmware**. The **Firmware** tab shows the current {{< product-c8y-iot >}} Edge version.

   ![Edge version](/images/edge-k8s/edge-k8s-firmware-current-version.png)

   You can also see the current {{< product-c8y-iot >}} Edge version in the **Info** tab.

   ![Edge version](/images/edge-k8s/edge-k8s-firmware-version-info-tab.png)

6. Click **Replace firmware**.

7. Select the firmware that you just uploaded and click **Install**.
   ![Edge version](/images/edge-k8s/edge-k8s-select-firmware.png)

   - To check the status of the update, hover over the refresh icon as shown in the figure below:
   ![Edge version](/images/edge-k8s/edge-k8s-check-remote-update-status.png)
   - To check the details of the update, click the text outlined in red in the figure below:
   ![Edge version](/images/edge-k8s/edge-k8s-check-remote-update-full-log.png)

### Updating Edge appliances using bulk operations {#updating-edge-appliances-using-bulk-operations}

For information about updating {{< product-c8y-iot >}} Edge using bulk operations, see [Updating {{< product-c8y-iot >}} Edge using bulk operations](/edge/edge-connectivity/#updating-edge-appliances-using-bulk-operations).
