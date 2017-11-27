# rhsatellite_install_master

## Description:

Install an instance of RedHat Satellite 6 along with minimum configuration
(See role xxxx for additional configuration role)

_Note: Still work in progress_

## Behaviour:

**Feature:** Installs a Satellite 6 server  
- **Given** a VM of capable size and power is available
- **Given** the connection details to the VM are known
- **Given** valid RedHat subscription is available
- **When** the deployment is executed
- **Then** subscriptions are attached
- **Then** pre-requisite checks are run ()
- **Then** TBC



## Configuration:

A list of the external variables used by the role.

| Variable  | Description  | Example  | 
|---|---|---|
| **var1**  | Var1 description  |  Var1 example. |
| **var2**  |   |   |
| **var3**  |   |   |


## Usage:

How to invoke the role from a playbook:

```yaml
- name: Creates Tenant
  include_role:
    name: OpenShift_Create_Tenant
  vars:
    var1: '???'
    var2: '???'
    var3: '???'
```