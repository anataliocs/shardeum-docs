---
title: Hosted Deployment
sidebar_position: 4
---

# Deploy a Validator Node Instance to Spheron

1. Sign up for a [Spheron account](https://app.spheron.network/#/signup)
2. Navigate to our [Shardeum Testnet Validator Template](https://app.spheron.network/#/compute/marketplace?template=Shardeum%20Testnet%20Validator) on our Marketplace.
3. Click the "Use Template" button and Spheron will auto-configure the settings you need to deploy a Shardeum Testnet Validator.
4. Change the region that your instance will deploy to if desired.
5. Be sure to set your password then click "Deploy"

## Customize the Node Settings

Now to stake and activate your validator, we have to manually update a couple of things specific to your instance.

Check out this [Spheron article for details on this process with screenshots](https://blog.spheron.network/deploy-and-stake-a-shardeum-validator-on-spheron-in-minutes) and additional context.

### Update Instance Settings

On the Port Policy Info section of the instance dashboard, you will find mappings between Internal and External ports.

Grab the external port mappings that map to internal ports 9001 and 10001.

Click the "Settings" tab then click the "Update Instance" button.

In the "Template Configuration" section update the following parameters:
- `SHMEXT`:  _External Port mapped to internal port 9001_
- `SHMINT`:  _External Port mapped to internal port 10001_

Then click update.

### Access Validator GUI

On your instance dashboard, grab your Connection URL which maps from the internal port, 8080.

Example:  `provider.us-west.spheron.wiki:32003`

Then append `https://` to the connection URL and enter it into your browser.

Example:  https://provider.us-west.spheron.wiki:32003/

From this point you can follow the standard steps to connect your wallet and stake SHM to your validator 
detailed here on the [Run Validator page](https://docs.shardeum.org/node/run/validator#step-5-start-validator)


