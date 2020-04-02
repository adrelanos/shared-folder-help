# Makes setting up a shared folder for virtual machines a bit easier #

A metapackage, that creates a folder /mnt/shared with chmod 777, adds a group
"vboxsf", adds user "user" to group "vboxsf". Facilitates auto-mounting of
shared folders.

Currently only helps using shared folders with VirtualBox a bit easier (as in
requiring fewer manual steps from the user). Might in future make use of other
virtual machine's shared folders easier.
## How to install `shared-folder-help` using apt-get ##

1\. Download [Whonix's Signing Key]().

```
wget https://www.whonix.org/patrick.asc
```

Users can [check Whonix Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key) for better security.

2\. Add Whonix's signing key.

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg add ~/patrick.asc
```

3\. Add Whonix's APT repository.

```
echo "deb https://deb.whonix.org buster main contrib non-free" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `shared-folder-help`.

```
sudo apt-get install shared-folder-help
```

## How to Build deb Package from Source Code ##

Can be build using standard Debian package build tools such as:

```
dpkg-buildpackage -b
```

See [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/shared-folder-help). (Replace `package-name` with the actual name of this package.)

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`shared-folder-help` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
