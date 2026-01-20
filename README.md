# AIDefense-ReadOnly-Roles


## GCP
Run the following command from a cloud terminal in the GCP project that you wish to onboard
```
bash <( curl -Ls https://raw.githubusercontent.com/jlunde-cisco/AIDefense-ReadOnly-Roles/refs/heads/main/gcp-read-only.sh ) -p ciscomcd -w "https://prod1-webhook.mcd.us.cdo.cisco.com:8093/webhook/CDO_cisco-aidefensesedemo__stc00d/gcp"

```
1.  Open Multicloud Defense in Cisco Security Cloud Control and select Home >> Easy Setup >> Connect Account >> GCP
2.  Once complete use the values to fill in the form within Multicloud Defense
3. If you want to populate External Visibility within AI Defense, navigate to Home >> Easy Setup >> Enable Traffic Visibility and enable visibility for the VPC's you want to capture VPC flow logs, and DNS query logs for.

## Azure
Run the following command from a cloud terminal in the Azure subscription you wish to onboard
```
bash <( curl -Ls https://raw.githubusercontent.com/jlunde-cisco/AIDefense-ReadOnly-Roles/refs/heads/main/azure-read-only.sh) -w "https://prod1-webhook.mcd.us.cdo.cisco.com:8093/webhook/CDO_cisco-aidefensesedemo__stc00d/azure"
```
1.  Open Multicloud Defense in Cisco Security Cloud Control and select Home >> Easy Setup >> Connect Account >> Azure
2.  Once complete use the values to fill in the form within Multicloud Defense

## AWS
Download the **aws-read-only-cf.yaml** file, and import it into your AWS enviornments cloudformation through the 'Create Stack' option. 
1.  Open Multicloud Defense in Cisco Security Cloud Control and select Home >> Easy Setup >> Connect Account
2.  Select AWS and copy the external ID (you will need this later)
3.  Copy this Cisco AWS Account number: **878511901175** (you will need this later)
4.  Fill in, and deploy the Cloud Formation Template
5.  Once complete navigate to the outputs tab, and use the values to fill in the form within Multicloud Defense
6. If you want to populate External Visibility within AI Defense, navigate to Home >> Easy Setup >> Enable Traffic Visibility and enable visibility for the VPC's you want to capture VPC flow logs, and DNS query logs for.
