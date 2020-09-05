# Everyday ARM template catalog

Welcome to my everyday ARM template catalog. This repo includes of templates where I could have spend some time on to 'invent' on how to do it. They all have some sort of use case behind them.

## Use cases
---

### Deploy a single vnet with multiple subnets, which have different settings, from a parameter file
Story behind this: ever wondered how to deploy a single vnet in ARM that has multiple subnets but those subnets would have different settings? For example, you would want that some subnets have NSG's or route tables but not all of them? (Like gatewaysubnet or something). This is a template that does exactly that. All subnet specific settings go in a parameter file and if the properties securityRules and routingRules are empty it will not assign a nsg or route table.

Fun fact: this use case finally showed me that functions in ARM can be usefull after all.

---
Currently working on 1 other use case