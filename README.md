> Wallpapers created by me using [SlackWall](https://forge.slackware.nl/rizitis/SlackWall) scripts 

# plasma-wallpapers

KDE Plasma wallpapers rendered with [SlackWall](https://forge.slackware.nl/rizitis/SlackWall).

Every folder is a complete Plasma wallpaper package with light and dark
variants in resolutions from 1920x540 up to 7680x5760.

**This repository is very large (several GB). Do not `git clone` it
normally.** Pick the wallpapers you want from the previews below and
download only those, as shown next.

## Download only the wallpapers you want

Requires git 2.27 or newer.

**1. Clone the repository without the wallpapers** (a few hundred KB):

```bash
git clone --depth 1 --filter=blob:none --sparse https://github.com/rizitis/plasma-wallpapers.git
cd plasma-wallpapers
```

**2. Choose the folders.** Use the folder names from the previews below:

```bash
git sparse-checkout set slackwall-blobs-326362582 slackwall-knots-1575146810
```

Only those folders are downloaded. Each one is roughly 150-600 MB.

To list all available folders from inside the clone:

```bash
git ls-tree -d --name-only HEAD
```

**Add more later** (keeps the ones you already have):

```bash
git sparse-checkout add slackwall-cloud-759497691
```

**Replace your selection** (folders not listed are removed from disk):

```bash
git sparse-checkout set slackwall-silk-749016951
```

**Get new wallpapers or updates** for your selection:

```bash
git pull
```

## Install in Plasma

Copy the folders into your local wallpapers directory:

```bash
mkdir -p ~/.local/share/wallpapers
cp -r slackwall-*/ ~/.local/share/wallpapers/
```

For all users, copy them to `/usr/share/wallpapers/` as root instead.

Then right click the desktop, choose **Configure Desktop and Wallpaper**,
and the new wallpapers appear in the list. Plasma picks the resolution
that matches your screen and switches to the dark variant when you use a
dark color scheme.

## Folder layout

```
slackwall-NAME-SEED/
├── metadata.json
└── contents/
    ├── screenshot.png
    ├── images/          light variant, all resolutions
    └── images_dark/     dark variant, all resolutions
```

## Previews

|   |   |   |
|---|---|---|
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-bars-1328263361/contents/screenshot.png" width="260"><br>`slackwall-bars-1328263361` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-blobs-326362582/contents/screenshot.png" width="260"><br>`slackwall-blobs-326362582` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-city-bluehour-aerial-1503273170/contents/screenshot.png" width="260"><br>`slackwall-city-bluehour-aerial-1503273170` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-city-night-aerial-1465435221/contents/screenshot.png" width="260"><br>`slackwall-city-night-aerial-1465435221` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-city-night-aerial-544553971/contents/screenshot.png" width="260"><br>`slackwall-city-night-aerial-544553971` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-city-night-rooftop-249009477/contents/screenshot.png" width="260"><br>`slackwall-city-night-rooftop-249009477` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-cloud-759497691/contents/screenshot.png" width="260"><br>`slackwall-cloud-759497691` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-diorama-autumn-1670216078/contents/screenshot.png" width="260"><br>`slackwall-diorama-autumn-1670216078` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-diorama-autumn-499331415/contents/screenshot.png" width="260"><br>`slackwall-diorama-autumn-499331415` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-diorama-meadow-1631760197/contents/screenshot.png" width="260"><br>`slackwall-diorama-meadow-1631760197` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-folds-1337768984/contents/screenshot.png" width="260"><br>`slackwall-folds-1337768984` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-folds-2061081494/contents/screenshot.png" width="260"><br>`slackwall-folds-2061081494` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-folds-503684299/contents/screenshot.png" width="260"><br>`slackwall-folds-503684299` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-folds-541836218/contents/screenshot.png" width="260"><br>`slackwall-folds-541836218` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-knots-1255580737/contents/screenshot.png" width="260"><br>`slackwall-knots-1255580737` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-knots-1575146810/contents/screenshot.png" width="260"><br>`slackwall-knots-1575146810` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-knots-1899852606/contents/screenshot.png" width="260"><br>`slackwall-knots-1899852606` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-knots-327518546/contents/screenshot.png" width="260"><br>`slackwall-knots-327518546` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-landscape-alien-2015495370/contents/screenshot.png" width="260"><br>`slackwall-landscape-alien-2015495370` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-landscape-alpine-1451720918/contents/screenshot.png" width="260"><br>`slackwall-landscape-alpine-1451720918` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-landscape-arctic-386126082/contents/screenshot.png" width="260"><br>`slackwall-landscape-arctic-386126082` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-landscape-desert-1292392465/contents/screenshot.png" width="260"><br>`slackwall-landscape-desert-1292392465` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-landscape-islands-774521012/contents/screenshot.png" width="260"><br>`slackwall-landscape-islands-774521012` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-ocean-day-291314497/contents/screenshot.png" width="260"><br>`slackwall-ocean-day-291314497` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-pile-698171483/contents/screenshot.png" width="260"><br>`slackwall-pile-698171483` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-plates-685793698/contents/screenshot.png" width="260"><br>`slackwall-plates-685793698` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-prisms-1308219530/contents/screenshot.png" width="260"><br>`slackwall-prisms-1308219530` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-prisms-658826976/contents/screenshot.png" width="260"><br>`slackwall-prisms-658826976` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-ribbons-1891368685/contents/screenshot.png" width="260"><br>`slackwall-ribbons-1891368685` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-rings-1751827165/contents/screenshot.png" width="260"><br>`slackwall-rings-1751827165` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-rings-470076065/contents/screenshot.png" width="260"><br>`slackwall-rings-470076065` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-scatter-1259078177/contents/screenshot.png" width="260"><br>`slackwall-scatter-1259078177` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-scatter-1548081209/contents/screenshot.png" width="260"><br>`slackwall-scatter-1548081209` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-scatter-224434988/contents/screenshot.png" width="260"><br>`slackwall-scatter-224434988` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-scatter-979064197/contents/screenshot.png" width="260"><br>`slackwall-scatter-979064197` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-scatter-984937884/contents/screenshot.png" width="260"><br>`slackwall-scatter-984937884` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-silk-1575308752/contents/screenshot.png" width="260"><br>`slackwall-silk-1575308752` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-silk-749016951/contents/screenshot.png" width="260"><br>`slackwall-silk-749016951` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-space-earth-1493208896/contents/screenshot.png" width="260"><br>`slackwall-space-earth-1493208896` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-space-earth-1934364184/contents/screenshot.png" width="260"><br>`slackwall-space-earth-1934364184` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-space-lava-77503206/contents/screenshot.png" width="260"><br>`slackwall-space-lava-77503206` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-spheres-1545635549/contents/screenshot.png" width="260"><br>`slackwall-spheres-1545635549` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-spheres-227407839/contents/screenshot.png" width="260"><br>`slackwall-spheres-227407839` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-spheres-302716582/contents/screenshot.png" width="260"><br>`slackwall-spheres-302716582` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-synthwave-1254823173/contents/screenshot.png" width="260"><br>`slackwall-synthwave-1254823173` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-synthwave-542369145/contents/screenshot.png" width="260"><br>`slackwall-synthwave-542369145` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-synthwave-974797688/contents/screenshot.png" width="260"><br>`slackwall-synthwave-974797688` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-tubes-1406522509/contents/screenshot.png" width="260"><br>`slackwall-tubes-1406522509` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-tubes-558993130/contents/screenshot.png" width="260"><br>`slackwall-tubes-558993130` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-voxel-1608928566/contents/screenshot.png" width="260"><br>`slackwall-voxel-1608928566` | <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-voxel-2071423218/contents/screenshot.png" width="260"><br>`slackwall-voxel-2071423218` |
| <img src="https://raw.githubusercontent.com/rizitis/plasma-wallpapers/refs/heads/main/slackwall-voxel-758680489/contents/screenshot.png" width="260"><br>`slackwall-voxel-758680489` |   |   |

## License

See [LICENSE](LICENSE).

