![Laravel Nova Localization Logo](./logo.png)

This repository is like Babbel for your [Laravel Nova](https://nova.laravel.com) app, without the learning part. It's a curated list of more than twenty language files for your favorite admin panel. Big thanks to all the great worldwide contributors.

---

## Available languages (21 languages)

| Code | LCID | Language | Thanks to |
| ------------- | ------------- | ------------- | ------------- |
| **ar**  |  | Arabic | [hanikeddah](https://github.com/hanikeddah)  |
| **bn**  |  | Bengali | [iamazik](https://github.com/iamazik) |
| **da**  |  | Danish | [peterbrinck](https://github.com/peterbrinck) |
| **de** | de-de | German | [franzdumfart](https://github.com/franzdumfart), [mrmonat](https://github.com/mrmonat), [pajoda](https://github.com/pajoda) |
| **en**  | en-us | English | Nova folks |
| **es**  | es-es | Spanish | [tinthenet](https://github.com/tinthenet), [Zerquix18](https://github.com/Zerquix18) and [driade](https://github.com/driade) |
| **fr**  |  | French | [xel1045](https://github.com/xel1045) and [benjamincrozat](https://github.com/benjamincrozat) |
| **gr**  |  | Greek | [Erth0](https://github.com/Erth0) |
| **id**  |  | Indonesian | [mul14](https://github.com/mul14) and [zeroseed](https://github.com/zeroseed) |
| **it**  |  | Italian | [s3b4stian](https://github.com/s3b4stian) |
| **lt**  |  | Lithuanian | [s3b4stian](https://github.com/s3b4stian) |
| **nb** | no-no | Norwegian | [LasseHaslev](https://github.com/LasseHaslev) |
| **nl**  |  | Netherlands | [Cannonb4ll](https://github.com/Cannonb4ll) and [patrickbergman](https://github.com/patrickbergman) |
| **pl**  |  | Polish | [aurawindsurfing](https://github.com/aurawindsurfing) |
| **pt**  | 	pt-br | Portuguese (Brazil) | [dessimoni](https://github.com/dessimoni) |
| **ru**  |  | Russian | [SerhiiStarovoitov](https://github.com/SerhiiStarovoitov) |
| **sq**  |  | Albanian | [sallmin](https://github.com/sallmin) |
| **tl**  |  | Tagalog | [ambengers](https://github.com/ambengers) |
| **tr**  |  | Turkish | [emir](https://github.com/emir) |
| **uk**  |  | Ukrainian | [ustych](https://github.com/ustych) |
| **zh**  | zh-cn | Chinese (China) | [jltxwesley](https://github.com/jltxwesley) |


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
