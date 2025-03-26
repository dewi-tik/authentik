---
title: Integrate with Wazuh
sidebar_label: Wazuh
support_level: community
---

## What is Wazuh

> Wazuh is a free and open source platform used for threat prevention, detection, and response. It is capable of protecting workloads across on-premises, virtualized, containerized, and cloud-based environments.
>
> -- https://github.com/wazuh/wazuh

## Preparation

The following placeholders are used in this guide:

- `wazuh.company` is the FQDN of the Wazuh installation. (Remove this for SaaS)
- `authentik.company` is the FQDN of the authentik installation.

:::note
This documentation lists only the settings that you need to change from their default values. Be aware that any changes other than those explicitly mentioned in this guide could cause issues accessing your application.
:::

## authentik configuration

To support the integration of _Wazuh_ with authentik, you need to create an application/provider pair in authentik.

_Any specific info about this integration can go here._

### Create an application and provider in authentik

1. Log in to authentik as an admin, and open the authentik Admin interface.
2. Navigate to **Applications** > **Applications** and click **Create with Provider** to create an application and provider pair. (Alternatively you can create only an application, without a provider, by clicking **Create**.)

- **Application**: provide a descriptive name, an optional group for the type of application, the policy engine mode, and optional UI settings.
    - _If there are any specific settings required, list them here. Refer to the [ownCloud integration documentation](https://github.com/goauthentik/authentik/blob/main/website/integrations/services/owncloud/index.md) for a complex requirements example._
- **Choose a Provider type**
    - _If there is a specific provider type required, state that here._
- **Configure the Provider**: provide a name (or accept the auto-provided name), the authorization flow to use for this provider, and the following required configurations.
    - _If there are any specific settings required, list them here. Refer to the [ownCloud integration documentation](https://github.com/goauthentik/authentik/blob/main/website/integrations/services/owncloud/index.md) for a complex requirements example._
- **Configure Bindings** _(optional)_: you can create a [binding](/docs/add-secure-apps/flows-stages/bindings/) (policy, group, or user) to manage the listing and access to applications on a user's **My applications** page.

3. Click **Submit** to save the new application and provider.

## Wazuh configuration

Insert Service configuration

1. Write first step here...

2. Continue with steps....

## Configuration verification

Template sentence that you can typically use here: "To confirm that authentik is properly configured with _Wazuh_, log out and log back in via authentik."

If there are more specific validation methods for the Service (e.g., clicking a button), include these instructions for clarity.
