# ScafL - Steam Card Afk Farm for Linux Flatpak

My current progress on the flatpak version of ScafL. Unfortunately I couldn't get libsteam to detect a Steam process. The rest of the application seems to work.

To build the application, you need org.gnome.Sdk and org.gnome.Platform versions 41 installed. You also need flatpak-builder.

```sh
flatpak install org.gnome.Sdk org.gnome.Platform
```

To build the flatpak, run:

```sh
flatpak-builder build-dir io.github.ScafL.yml
```

After finishing the build process, you can run the application with the following command

```sh
flatpak-builder --run build-dir io.github.ScafL.yml scafl
```