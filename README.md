Role Name
========

Ansible role to install Sysdig. Sysdig is a system-level exploration tool: capture system state and activity from a running Linux instance, then save, filter and analyze.

Requirements
------------

None

Role Variables
--------------

`sysdig_epel_6: "http://dl.fedoraproject.org/pub/epel/6/x86_64/epel-release-6-8.noarch.rpm"`

`sysdig_epel_7: "http://dl.fedoraproject.org/pub/epel/beta/7/x86_64/epel-release-7-0.2.noarch.rpm"`

`sysdig_repokey: "https://s3.amazonaws.com/download.draios.com/DRAIOS-GPG-KEY.public"`

`sysdig_url: "http://download.draios.com/stable/rpm/draios.repo"`

`sysdig_repo: "/etc/yum.repos.d/draios.repo"`

`sysdig_package: "sysdig"`

`sysdig_url_apt: "http://download.draios.com/stable/deb/draios.list"`

`sysdig_repo_apt: "/etc/apt/sources.list.d/draios.list"`

Dependencies
------------

None

Example Playbook
-------------------------

    - hosts: sysdigs
      roles:
         - { role: valentinogagliardi.sysdig,
                   tags: ["sysdig"] }

License
-------

GNU General Public License Version 2

Author Information
------------------

Valentino Gagliardi - valentino.g [at] servermanaged.it
