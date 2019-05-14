# Laravel Nova Localizations

![Laravel Nova Localization Logo](./logo.png)

This repository is like Babbel for your [Laravel Nova](https://nova.laravel.com) app, without the learning part. It's a curated list of nearly thirty language files for your favorite admin panel. Big thanks to all the great worldwide contributors.

[![StyleCI Status](https://github.styleci.io/repos/145764698/shield)](https://github.styleci.io/repos/145764698)

---

## Available languages (29 languages)

| Language | Code | LCID | Thanks to |
| :--- | ------------- | ------------- | :--- |
| Albanian  | **sq** |  | [sallmin](https://github.com/sallmin) |
| Arabic  | **ar** | ar-sy | [Danyel Alkeddah](https://github.com/K3DVII)  |
| Azeri | **az** | az-az | [Energon7](https://github.com/Energon7) |
| Bengali  | **bn** | bn-bd | [iamazik](https://github.com/iamazik) |
| Catalan  | **ca** | es-ca | [lloople](https://github.com/lloople) |
| Chinese (China) | **zh** | zh-cn | [jltxwesley](https://github.com/jltxwesley), [yangliulnn](https://github.com/yangliulnn), [nighon](https://github.com/nighon) |
| Chinese (Traditional)  | **zh** | zh-tw | [tinghom](https://github.com/tinghom), [yangliulnn](https://github.com/yangliulnn) |
| Danish  | **da** |  | [peterbrinck](https://github.com/peterbrinck) |
| Dutch  | **nl** |  | [Cannonb4ll](https://github.com/Cannonb4ll), [patrickbergman](https://github.com/patrickbergman), [DannyStreur](https://github.com/DannyStreur), [ovvessem](https://github.com/ovvessem) |
| English  | **en** | en-us | Nova folks |
| Finnish  | **fi** |  | [joonas1234](https://github.com/joonas1234), [SirMathays](https://github.com/SirMathays) |
| French  | **fr** | fr-fr | [xel1045](https://github.com/xel1045), [benjamincrozat](https://github.com/benjamincrozat), [electronick86](https://github.com/electronick86) |
| German | **de** | de-de | [franzdumfart](https://github.com/franzdumfart), [mrmonat](https://github.com/mrmonat), [pajoda](https://github.com/pajoda), [dastiii](https://github.com/dastiii), [hofmannsven](https://github.com/hofmannsven) |
| Greek  | **gr** |  | [Erth0](https://github.com/Erth0) |
| Hungarian  | **hu** |  | [milli05](https://github.com/milli05), [drobee](https://github.com/drobee) |
| Indonesian  | **id** |  | [mul14](https://github.com/mul14), [zeroseed](https://github.com/zeroseed) |
| Italian  | **it** | it-it | [s3b4stian](https://github.com/s3b4stian) |
| Korean  | **ko** |  | [getsolaris](https://github.com/getsolaris) |
| Lithuanian  | **lt** |  | [girvydas](https://github.com/girvydas), [Justas Maziliauskas](https://github.com/justutiz) |
| Norwegian | **nb** | nb-no | [LasseHaslev](https://github.com/LasseHaslev), [Marcuzz](https://github.com/Marcuzz) |
| Persian (Farsi)  | **fa** |  | [mehranhadidi](https://github.com/mehranhadidi) |
| Polish  | **pl** |  | [aurawindsurfing](https://github.com/aurawindsurfing), [JackShev](https://github.com/JackShev) |
| Portuguese (Brazil)  | **pt** | pt-br | [dessimoni](https://github.com/dessimoni) |
| Portuguese (Portugal) | **pt** | pt-pt | [sikrew](https://github.com/sikrew) |
| Russian  | **ru** | ru | [SerhiiStarovoitov](https://github.com/SerhiiStarovoitov), [mexoboy](https://github.com/mexoboy) |
| Slovenian  | **sl** | sl | [morpheus7CS](https://github.com/morpheus7CS), [squierll](https://github.com/squierll) |
| Spanish  | **es** | es-es | [tinthenet](https://github.com/tinthenet), [Zerquix18](https://github.com/Zerquix18), [driade](https://github.com/driade), [kennyhorna](https://github.com/kennyhorna) |
| Tagalog  | **tl** |  | [ambengers](https://github.com/ambengers) |
| Turkish  | **tr** |  | [emir](https://github.com/emir), [EnesCakir](https://github.com/EnesCakir) |
| Ukrainian  | **uk** |  | [ustych](https://github.com/ustych), [igorbabko](https://github.com/igorbabko) |

## Usage

### Manual

Navigate to the `lang` folder, download your preferred language files, save them to `/resources/lang/vendor/nova/`.
For further details about Nova Localization, please check out [the docs](https://nova.laravel.com/docs/1.0/customization/localization.html).

### Automatic

You can make sure that you are always up to date with the latest translations by adding two commands on the `post-autoload-dump` hook in your `composer.json` file. Of course, you can do that for as many languages as you want.

```json
{
    "scripts": {
        "pre-update-cmd": [
            "@php -r \"mkdir('./resources/lang/vendor/nova', 0776, true);\"",
            "@php -r \"copy('https://raw.githubusercontent.com/franzdumfart/laravel-nova-localizations/master/lang/fr.json', './resources/lang/vendor/nova/fr.json') || exit (1);\""
        ],
        "post-autoload-dump": [
            "..."
        ]
    },
}
```

Don't forget to customize for your needs.

## Help

Feel free to submit a pull request, add your desired language or updates.
