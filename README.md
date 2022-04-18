<p align="center">
	<img src="com.github._0negal.Viper.png" width="200px"><br>
</p>

# Viper

Viper is a launcher and updater for [Northstar](https://github.com/R2Northstar/Northstar), and not much more than that.

The Flatpak version simply takes the upstream tar archive and repacks it inside a Flatpak sandbox.

The repository for Viper can be found [here](https://github.com/0neGal/viper).

## Flatpak specific issues

If the install location for Titanfall2 is not within either your home directory, `/media` (usual location for SD cards), or `/mnt` (usual location for additional drives), Viper will be unable to locate it due to restricted filesystem access imposed by the Flatpak sandbox.

If this applies to you, you can manually give the Flatpak version of Viper full filesystem access using either [Flatseal](https://flathub.org/apps/details/com.github.tchx84.Flatseal) or via the command line:

```
flatpak override com.github._0negal.Viper --filesystem=host
```
