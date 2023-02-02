# `Iuliia`

> Transliterate Cyrillic → Latin in every possible way

this fork append:
> Transliterate Latin -> Cirilic with support the native translation some words

Transliteration means representing Cyrillic data (mainly names and geographic locations) with Latin letters. It is used for international passports, visas, green cards, driving licenses, mail and goods delivery etc.

## Installation
Maven dependency
```xml
<!-- https://mvnrepository.com/artifact/ru.homyakin/iuliia-java -->
<dependency>
    <groupId>ru.homyakin</groupId>
    <artifactId>iuliia-java</artifactId>
    <version>1.8</version>
</dependency>
```

Gradle
```gradle
implementation 'ru.homyakin:iuliia-java:1.8'
```

## Usage (Java 11 and higher)

Transliterate using specified schema:

```java
import ru.homyakin.iuliia.Schemas;
import ru.homyakin.iuliia.Translator;

public class Clazz {
    public static void test() {        
        var translator = new Translator(Schemas.ICAO_DOC_9303);
        translator.translate("Юлия"); //Iuliia
    }
}
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Make sure to add or update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
