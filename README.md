# Dynatrace-Fixpack-Ansible

An [Ansible](http://www.ansible.com) role for automated deployments of a [Dynatrace](http://bit.ly/dttrial) Fixpack. 

**Note**: Currently, we support only Linux hosts, support for installing Windows hosts is in the making.

## Download

The role is available via:

- [Ansible Galaxy](https://galaxy.ansible.com/list#/roles/2627)
- [GitHub](https://github.com/Dynatrace/Dynatrace-Fixpack-Ansible)

## Requirements

Place a fixpack as ```dynatrace-fixpack.dtf``` in the role's ```files``` directory from where it will be picked up during the automated installation.

## Role Variables

As defined in ```defaults/main.yml```:

| Name                                            | Default                                          | Description |
|-------------------------------------------------|--------------------------------------------------|-------------|
| *dynatrace_fixpack_file_name*                   | dynatrace-fixpack.dtf                            | The file name of the Dynatrace Fixpack in the role's ```files``` directory. |
| *dynatrace_fixpack_file_url*                    | http://localhost/dynatrace/dynatrace-fixpack.dtf | A HTTP, HTTPS or FTP URL to the Dynatrace Fixpack in the form (http\|https\|ftp)://[user[:pass]]@host.domain[:port]/path. |
| *dynatrace_fixpack_user_name*                   | admin                                            | The username of a Dynatrace user that has the *Manage Fixpacks* permission. |
| *dynatrace_fixpack_user_password*               | admin                                            | The password of a Dynatrace user that has the *Manage Fixpacks* permission. |
| *dynatrace_fixpack_role_name*                   | dynatrace.Dynatrace-Fixpack                      | The actual name of this role in an [Ansible Playbook's](http://docs.ansible.com/playbooks.html) ```roles``` directory. |

## Example Playbook

	- hosts: all
	  roles:
	    - role: dynatrace.Dynatrace-Fixpack

## Additional Resources

- [Blog: How to Automate Enterprise Application Monitoring with Ansible](http://apmblog.dynatrace.com/2015/03/04/how-to-automate-enterprise-application-monitoring-with-ansible/)
- [Blog: How to Automate Enterprise Application Monitoring with Ansible - Part II](http://apmblog.dynatrace.com/2015/04/23/how-to-automate-enterprise-application-monitoring-with-ansible-part-ii/)
- [Slide Deck: Automated Deployments](http://slideshare.net/MartinEtmajer/automated-deployments-slide-share)
- [Slide Deck: Automated Deployments (of Dynatrace) with Ansible](http://www.slideshare.net/MartinEtmajer/automated-deployments-with-ansible)
- [Slide Deck: Testing Ansible Roles with Test Kitchen, Serverspec and RSpec](http://www.slideshare.net/MartinEtmajer/testing-ansible-roles-with-test-kitchen-serverspec-and-rspec-48185017)
- [Tutorials: Automated Deployments (of Dynatrace) with Ansible](https://community.compuwareapm.com/community/display/COE/Tutorials+on+Automated+Deployments#TutorialsonAutomatedDeployments-ansible)

## Questions?

Feel free to post your questions on the Dynatrace Community's [Continuous Delivery Forum](https://community.dynatrace.com/community/pages/viewpage.action?pageId=46628921).

## License

Licensed under the MIT License. See the LICENSE file for details.
[![analytics](https://www.google-analytics.com/collect?v=1&t=pageview&_s=1&dl=https%3A%2F%2Fgithub.com%2FdynaTrace&dp=%2FDynatrace-Fixpack-Ansible&dt=Dynatrace-Fixpack-Ansible&_u=Dynatrace~&cid=github.com%2FdynaTrace&tid=UA-54510554-5&aip=1)]()