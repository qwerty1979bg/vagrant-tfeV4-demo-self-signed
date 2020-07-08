# vagrant-tfeV4-demo-self-signed

task: Install DEMO version of Terraform Enterprise (ex PTFE) v4 with Self Signed Certificate - Vagrant

## Usage

1. [Install Vagrant](https://www.vagrantup.com/docs/installation/)
2. Clone this repository and `cd` into it.

3. Run the following:

```
$ vagrant plugin install vagrant-disksize
$ vagrant up

* open a web browser to http://localhost:8800/
* Continue the manual set-up according to the guide

When done, do a
$ vagrant destroy
```

* [Installation instructions](https://www.terraform.io/docs/enterprise/install/index.html) / [Pre-flight checklist](https://www.terraform.io/docs/enterprise/before-installing/index.html) / [Refference architecture](https://www.terraform.io/docs/enterprise/before-installing/reference-architecture/index.html)


[Deployment method](https://www.terraform.io/docs/enterprise/before-installing/index.html#deployment-method-decision): Individual deployment

[Operational mode](https://www.terraform.io/docs/enterprise/before-installing/index.html#operational-mode-decision): Demo

[Credentials](https://www.terraform.io/docs/enterprise/before-installing/index.html#operational-mode-decision): *TODO*

[Data storage](https://www.terraform.io/docs/enterprise/before-installing/index.html#data-storage): [Mounted disk](https://www.terraform.io/docs/enterprise/before-installing/disk-requirements.html#supported-mounted-disk-types)
(*note: not needed in DEMO mode*)

[Linux instance](https://www.terraform.io/docs/enterprise/before-installing/index.html#operating-system-requirements): Ubuntu 18.04

[Hardware requirements](https://www.terraform.io/docs/enterprise/before-installing/index.html#hardware-requirements)

Todo:

- [] 

Done:
- [*] create Vagrantfile with a Ubuntu Bionic VM
- [*] port forward 8800
- [*] At least 8GB of system memory
- [*] At least 2 CPU cores
- [*] At least 40GB of disk space on the root volume
- [*] SELinux set to permissive, to run TFE in DEMO mode - not needed, since this is not RedHat / CentOS
- [*] provision script to run TFE installer

