# Host Parameters

The templates use some Host Parameters to contol the flow of the template. These are:

* install-disk: What device to install to (default: /dev/sda | /dev/vda)
* ssh_authorized_keys: add public SSH keys which will be authorized for the core user. You can specify multiple SSH keys seperated with a "," (default: empty)
* etcd_discovery_url: provision a discovery token for etcd to allow a simple cluster deployment. You can get a new discovery token at [https://discovery.etcd.io/new](https://discovery.etcd.io/new). This parameter is used in the [coreos_cloudconfig snippet](https://github.com/theforeman/community-templates/blob/master/snippets/coreos_cloudconfig.erb). (default: empty)

More Information are available on the [CoreOS site](https://coreos.com/docs/cluster-management/setup/cloudinit-cloud-config)