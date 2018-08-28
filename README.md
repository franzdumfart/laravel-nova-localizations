![Laravel Nova Localization Logo](./logo.png)

This repository is like Babbel for your [Laravel Nova](https://nova.laravel.com) app, without the learning part. It's a curated list of more than twenty language files for your favorite admin panel. Big thanks to all the great worldwide contributors.

---

## Available languages (21 languages)

| Language | Code | LCID | Thanks to |
| :--- | ------------- | ------------- | :--- |
| Arabic  | **ar** |  | [hanikeddah](https://github.com/hanikeddah)  |
| Albanian  | **sq** |  | [sallmin](https://github.com/sallmin) |
| Bengali  | **bn** | bn-bd | [iamazik](https://github.com/iamazik) |
| Chinese (China)  | **zh** | zh-cn | [jltxwesley](https://github.com/jltxwesley) |
| Danish  | **da** |  | [peterbrinck](https://github.com/peterbrinck) |
| English  | **en** | en-us | Nova folks |
| French  | **fr** | fr-fr | [xel1045](https://github.com/xel1045) and [benjamincrozat](https://github.com/benjamincrozat) |
| German | **de** | de-de | [franzdumfart](https://github.com/franzdumfart), [mrmonat](https://github.com/mrmonat), [pajoda](https://github.com/pajoda) |
| Greek  | **gr** |  | [Erth0](https://github.com/Erth0) |
| Indonesian  | **id** |  | [mul14](https://github.com/mul14) and [zeroseed](https://github.com/zeroseed) |
| Italian  | **it** | it-it | [s3b4stian](https://github.com/s3b4stian) |
| Lithuanian  | **lt** |  | [girvydas](https://github.com/girvydas) |
| Netherlands  | **nl** |  | [Cannonb4ll](https://github.com/Cannonb4ll) and [patrickbergman](https://github.com/patrickbergman) |
| Norwegian | **nb** | no-no | [LasseHaslev](https://github.com/LasseHaslev) |
| Polish  | **pl** |  | [aurawindsurfing](https://github.com/aurawindsurfing) |
| Portuguese (Brazil)  | **pt** | pt-br | [dessimoni](https://github.com/dessimoni) |
| Russian  | **ru** | ru | [SerhiiStarovoitov](https://github.com/SerhiiStarovoitov) |
| Spanish  | **es** | es-es | [tinthenet](https://github.com/tinthenet), [Zerquix18](https://github.com/Zerquix18) and [driade](https://github.com/driade) |
| Tagalog  | **tl** |  | [ambengers](https://github.com/ambengers) |
| Turkish  | **tr** |  | [emir](https://github.com/emir) |
| Ukrainian  | **uk** | uk | [ustych](https://github.com/ustych) |

## Usage

### Manual
Navigate to the `lang` folder, download your preferred language files and save them to `/resources/lang/vendor/nova/`.
For further details about Nova Localization, please check out [the docs](https://nova.laravel.com/docs/1.0/customization/localization.html).

### Automatic
You can make sure that you are always up to date with the latest translations by adding two commands on the `post-autoload-dump` hook in your `composer.json` file. Of course, you can do that for as many languages as you want.

```json
{
    "scripts": {
        "post-autoload-dump": [
            "Illuminate\\Foundation\\ComposerScripts::postAutoloadDump",
            "@php artisan package:discover",
            "mkdir -p resources/lang/vendor/nova",
            "wget https://raw.githubusercontent.com/franzdumfart/laravel-nova-localizations/master/lang/fr.json -O resources/lang/vendor/nova/fr.json"
        ]
    },
}
```
Don't forget to customize for your needs.

## Help
Feel free to submit a pull request and add your desired language or updates.
