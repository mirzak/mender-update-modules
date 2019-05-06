## Description

The Directory Overlay Update Module installs a user defined file tree structure into a given destination directory in the target.

Before the deploy into the destination folder on the device, the Update Module will take a backup copy of the current contents, allowing restore of it using the rollback mechanism of the Mender client if something goes wrong. The Update Module will also delete the current installed content that was previously installed using the same module, this means that each deployment is self contained and there is no residues left on the system from the previous deployment.

Example use-cases:
* Deploy root filesystem overlays

## Specification

|||
| --- | --- |
|Module name| dir-overlay |
|Supports rollback|yes|
|Requires restart|no|
|Artifact generation script|yes|
|Full system updater|no|
|Source code|[Update Module](https://github.com/mirzak/dir-overlay/blob/master/modules/dir-overlay), [Artifact Generator](https://github.com/mirzak/dir-overlay/blob/master/modules-artifact-gen/dir-overlay-artifact-gen)|

For further details on usage see [Mender Hub](https://hub.mender.io/t/directory-overlay/)

## Maintainer

The author and maintainer of this Update Module is:

- Mirza Krak - <mirza.krak@northern.tech> - [mirzak](https://github.com/mirzak)

Always include the original author when suggesting code changes to this update module.
