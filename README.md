memoryleak.gradle
=================

Download and unzip Gradle.

Requirements
------------

None

Role Variables
--------------

	gradle_version: 6.2.2
	gradle_download_url: "https://services.gradle.org/distributions/gradle-{{ gradle_version }}-bin.zip"
	gradle_installation_parent: "{{ ansible_user_dir }}/.local/share/gradle"
	gradle_installation_parent_create: True
	gradle_installation_owner: "{{ ansible_user_id }}"
	gradle_installation_group: "{{ ansible_effective_group_id }}"


Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - name: memoryleak.gradle

License
-------

MIT

Author Information
------------------

Haydar Ciftci <haydar.ciftci@gmail.com>
