# Makes setting up a shared folder for virtual machines a bit easier #

A metapackage, that creates a folder /mnt/shared with chmod 777, adds a group
"vboxsf", adds user "user" to group "vboxsf". Facilitates auto-mounting of
shared folders.

Currently only helps using shared folders with VirtualBox a bit easier (as in
requiring fewer manual steps from the user). Might in future make use of other
virtual machine's shared folders easier.
## How to install `shared-folder-help` using apt-get ##

1\. Add [Whonix's Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key).

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg adv --keyserver hkp://ipv4.pool.sks-keyservers.net:80 --recv-keys 916B8D99C38EAF5E8ADC7A2A8D66066A2EEACCDA
```

3\. Add Whonix's APT repository.

```
echo "deb http://deb.whonix.org stretch main" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `shared-folder-help`.

```
sudo apt-get install shared-folder-help
```

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `shared-folder-help` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Payments ##

`shared-folder-help` requires [payments](https://www.whonix.org/wiki/Payments) to stay alive!
