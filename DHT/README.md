# DHT sensor library [![Build Status](https://github.com/adafruit/DHT-sensor-library/workflows/Arduino%20Library%20CI/badge.svg)](https://github.com/adafruit/DHT-sensor-library/actions)

## Description

An Arduino library for the DHT series of low-cost temperature/humidity sensors.

You can find DHT tutorials [here](https://learn.adafruit.com/dht).

Suitable for:  DHT11 / DHT12 / DHT21 / DHT22


## What the difference here ? 

Too often, the DHT driver has conflict with other Adafruit component's driver.
The variable sensor_t seams to be in every code.
That said, the following code provides a run around this problem, mostly when you want to connect new and old component all together onto a single project.
The following repository, also, includes the universal « Adafruit_sensor » file - renamed « Adafruit_sensorDHT » to make sure you have everything ready & easy to install.

This repository tends to avoid:
- 'error sensor_t' is all ready defined
- 'sensor_t' has not been declared
- 'AdafruitDHT_Sensor' has not been declared
- 'Adafruit_Sensor' already exists
- You can not redclare 'Adafruit_Sensor'
- 'AdafruitDHT_sensor_t' was not declared in this scope
- 'sensor' was not declared in this scope
- 'getSensor' was not declared in this scope

## Pourquoi encore un dépôt git pour DHT ? 
Trop souvent, les pilotes Adafruit utilisent les mêmes noms de variable et d'objet. Cela entraîne des conflit et des erreurs de compilation sous Arduino.
La variable passe-partout « sensor_t » utliisée dans les pilotes adafruit est changée ici à la faveur d'un nom unique « AdafruitDHT_sensor_t » de façon à éliminer ces conflits.
Vous trouverez donc ici un code, non pas amélioré, mais seulement modifié de façon à contourner ce problème de répétition.
De plus, le présent dépôt vous offre une version adaptée du pilote « Adafruit_sensor », renommé « Adafruit_sensorDHT » afin de vous assurer une installation facile et performante du premier coup.

Le présent dépôt devrait régler les problèmes suivants (selon les expressions originales anglaises de Arduino)
- 'error sensor_t' is all ready defined
- 'sensor_t' has not been declared
- 'AdafruitDHT_Sensor' has not been declared
- 'Adafruit_Sensor' already exists
- You can not redclare 'Adafruit_Sensor'
- 'AdafruitDHT_sensor_t' was not declared in this scope
- 'sensor' was not declared in this scope
- 'getSensor' was not declared in this scope


# Dependencies (optional)
As the Adafruit_universal driver is included in this deposite, you'd better use the one you find here.  Still, the original is ...
 * [Adafruit Unified Sensor Driver](https://github.com/adafruit/Adafruit_Sensor)


# Dépendances (facultatives)
Le présent dépôt inclut les fichiers modidfiés du dépôt Adafruit_unified_sensor.  Néanmoins, si vous souhaitez accéder aux fichiers originaux ...
 * [Adafruit Unified Sensor Driver](https://github.com/adafruit/Adafruit_Sensor)

# Contributing

Contributions are welcome!  Not only you’ll encourage the development of the library, but you’ll also learn how to best use the library and probably some C++ too
Please contribute to main project [Adafruit](https://github.com/adafruit/DHT-sensor-library/actions) and notice me about the needs of modifications here.

Please read our [Code of Conduct](https://github.com/adafruit/DHT-sensor-library/blob/master/CODE_OF_CONDUCT.md>)
before contributing to help this project stay welcoming.

## Documentation and doxygen
Documentation is produced by doxygen. Contributions should include documentation for any new code added.

Some examples of how to use doxygen can be found in these guide pages:

https://learn.adafruit.com/the-well-automated-arduino-library/doxygen

https://learn.adafruit.com/the-well-automated-arduino-library/doxygen-tips

Written by Adafruit Industries based on work by:

 * T. DiCola
 * P. Y. Dragon
 * L. Fried
 * J. Hoffmann
 * M. Kooijman
 * J. M. Dana
 * S. Conaway
 * S. IJskes
 * T. Forbes
 * B. C
 * T. J Myers
 * L. Sørup
 * per1234
 * O. Duffy
 * matthiasdanner
 * J. Lim
 * G. Ambrozio
 * chelmi
 * adams13x13
 * Spacefish
 * I. Scheller
 * C. Miller
 * 7eggert


MIT license, check license.txt for more information
All text above must be included in any redistribution

To install, use the Arduino Library Manager and search for "DHT sensor library" and install the library.
