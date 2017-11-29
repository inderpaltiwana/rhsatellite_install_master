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
- **Then** pre-requisite checks are run
- **Then** Red Hat Satellite is installed
- **Then** TBC



## Configuration:

A list of the external variables used by the role.

| Variable  | Description  | Example  | 
|---|---|---|
| **hostname**  | Host FQDN  |  satellite-x123456.mydomain.com |
| **satellite_admin_password**  |  Password for Satellite admin user |  |
| **satellite_initial_organization**  | Organisation name. | Default Organization |
| **satellite_initial_location**  | Initial location | Default Location |
| **satellite_proxy_url**  | Proxy server url (optional) | http://192.168.10.10  |
| **satellite_proxy_port**  | Proxy server port number (optional) | 3128  |
| **var3**  |   |   |


## Usage:

How to invoke the role from a playbook:

```yaml
- name: Installs Red Hat Satellite
  include_role:
    name: rhsatellite_install_master
  vars:
    hostname: 'satellite-x123456.mydomain.com'
    satellite_admin_password: 'f6E38KluywWK0ns'
    satellite_initial_organization: 'Widget and Gadget Co.'
    satellite_initial_location: 'United Kingdom'
    var3: '???'
```