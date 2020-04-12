# Phone Customization

## App list

Some of these are paid or have premium versions, but the KLWP can be manually configured from the free version  
Also, I like simple wallpapers ¯\\\_(ツ)\_/¯

* [Nova Launcher Prime](https://play.google.com/store/apps/details?id=com.teslacoilsw.launcher.prime&hl=en)
* [KLWP Live Wallpaper Maker](https://play.google.com/store/apps/details?id=org.kustom.wallpaper&hl=en)
* [KWGT Kustom Widget Maker](https://play.google.com/store/apps/details?id=org.kustom.widget&hl=en)
* [Whicons - White Icon Pack](https://play.google.com/store/apps/details?id=com.whicons.iconpack&hl=en)
* [RGB Color Wallpaper](https://play.google.com/store/apps/details?id=com.tecdrop.rgbwallpaper&hl=en)

## Scripts

Weather icon
```
$if( wf(icon, 0)=MCLOUDY, CLOUDY2,
wf(icon, 0)=CLEAR, SUN
)$
```
Date in Japanese format (Month then Day)
```
月$df(MM)$

日$df(d)$
```

Updating kanji fot the days of the week!
```
$if( df(EEEE)=Monday,月,
df(EEEE)=Tuesday, 火,
df(EEEE)=Wednesday,水 ,
df(EEEE)=Thursday,木,
df(EEEE)=Friday,金,
df(EEEE)=Saturday,土,
df(EEEE)=Sunday,日
)$
```

And the music player, in order
* Source (Youtube/Spotify/Audibook)

* Title of playing song/book/video

* Artist
```
[$tc(split, mi(package), ".", 1)$]

[i]$tc(ell, mi(title), 20)$[/i]

- $mi(artist)$ -
```

## Result

Current configuration

| Home        | Weather + Music Player  | App Drawer  |
|:-------------:|:-------------:|:-----:|
|![alt text](https://github.com/tinyAtlas/Phone_Customization/blob/master/Screenshot_20200412-135453.png "Screenshot 1")|![alt text](https://github.com/tinyAtlas/Phone_Customization/blob/master/Screenshot_20200412-135448.png "Screenshot 2")|![alt text](https://github.com/tinyAtlas/Phone_Customization/blob/master/Screenshot_20200412-140042.png "Screenshot 3")|


Samples from and older configuration

| Home        | Weather           | App Drawer  |
|:-------------:|:-------------:|:-----:|
|![alt text](https://github.com/tinyAtlas/Phone_Customization/blob/master/Screenshot_20200204-134509.png "Screenshot 1")|![alt text](https://github.com/tinyAtlas/Phone_Customization/blob/master/Screenshot_20200204-134523.png "Screenshot 2")|![alt text](https://github.com/tinyAtlas/Phone_Customization/blob/master/Screenshot_20200204-134718.png "Screenshot 3")|
