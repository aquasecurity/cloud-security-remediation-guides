[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / Scale Set Multi Az

## Quick Info

| | |
|-|-|
| **Plugin Title** | Scale Set Multi Az |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that Virtual Machine Scale Sets are created to be cross-AZ for high availability |
| **More Info** | Having Virtual Machine Scale Sets in multiple zones increases durability and availability. If there is a catastrophic instance in one zone, the scale set will still be available. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/virtual-machine-scale-sets-autoscale-overview |
| **Recommended Action** | Multiple zones can only be created when instantiating a new Scale Set. Ensure that the Scale Set is in multiple zones when creating a new Scale Set. |

## Detailed Remediation Steps


