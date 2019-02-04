# SamJSON
> UnrealEngine Graphs based JSON Library

SamJSON is a JSON Library that was created to be used by Modders of UnrealEngine based games like ARK and ATLAS where there is no access to the source code and all functionalities need to be implemented using the Blueprints Graphs System.

![](Screenshot_0.png)

## Features
* You can **Parse a JSON String into a SamJSON Object** and get all the Properties or Array Items from it using the provided _GetPropertyAsX/GetArrayAsX_ functions
* You can **Create a new empty SamJSON Object**, populate it with data using one of the _AddXProperty/AddXToArray_ functions and **generate a JSON string** out of it by calling _GetJSONString_
* You can **Change values of Properties** of a existing SamJSON object by using the provided _SetXProperty_ functions
* PrettyPrint - generate a nicely formated JSON string to print to logs, console or UI

![](Screenshot_2.png)

## Getting Started

These instructions will get you a copy of the assets needed to use samJSON in your own Mod Project.

### Prerequisites

UnrealEngine (Full or the DevKit of one of the supported games)

### Installing

* Clone or Download the assets from Git
* Copy the folder ArkZeroRP to your "Mods" folder so that you have the following structure "*/Game/Mods/ArkZeroRP/SamJSON/*"
* Start your Engine/DevKit and navigate to "/Game/Mods/ArkZeroRP/SamJSON" (you should see two Blueprints and two Folders)
* Done

### Asset List (BP - Blueprint)

* /ArkZeroRP/SamJSON/SamJSON.uasset - :red_circle:REQUIRED
  >The library BP based of Object
* /ArkZeroRP/SamJSON/SamJSON_ExampleSingleton.uasset - :large_blue_circle:OPTIONAL
  >Examples singleton BP based of Actor
* /ArkZeroRP/SamJSON/Enums/SamJSON_DataType.uasset - :red_circle:REQUIRED
  >Enum BP, possible types of Properties or Array Items
* /ArkZeroRP/SamJSON/Enums/SamJSON_ValueErrorType.uasset - :red_circle:REQUIRED
  >Enum BP, possible types of Errors when using GetPropertyAsX
* /ArkZeroRP/SamJSON/Structs/SamJSON_KeyValue.uasset - :red_circle:REQUIRED
  >Struct BP, represents a single property as Key/Value/Type
* /ArkZeroRP/SamJSON/Structs/Z_BoolMap.uasset - :red_circle:REQUIRED
  >Struct BP, represents a property as Key(String)/Value(Boolean) - Used for bulk adding of properties to a SamJSON object
* /ArkZeroRP/SamJSON/Structs/Z_NumberMap.uasset - :red_circle:REQUIRED
  >Struct BP, represents a property as Key(String)/Value(Float) - Used for bulk adding of properties to a SamJSON object
* /ArkZeroRP/SamJSON/Structs/Z_StringMap.uasset - :red_circle:REQUIRED
  >Struct BP, represents a property as Key(String)/Value(String) - Used for bulk adding of properties to a SamJSON object

### Usage example

* Open "SamJSON_ExampleSingleton" to see examples of how to use the "SamJSON" Blueprint that is the JSON Library itself
* (ARK/ATLAS)You can add "SamJSON_ExampleSingleton" to your singletons list in the PrimalGameData to execute it in PIE and see the examples in action

Parse a JSON String into SamJSON Object and query Properties
![](Screenshot_0.png)
![](Screenshot_1.png)

Create a new SamJSON Object and populate it with data
![](Screenshot_3.png)

## Release History

* 04.02.2019
    * CHANGE: Improvements to the README.md
* 02.02.2019
    * Full rework of the Library (more functional and organized)
	* FIX: Infinity Loops with nested arrays
	* FIX: Support for escaped characters
	* ADD: Example Singleton for testing the Library out and understanding how to use it
	* ADD: Tool-tips and Descriptions for all functions and variables as well as comments in the graphs where needed (Examples)
	* CHANGE: Categories of functions and variables for easier use and understanding

## Meta

**Samir (SamKO) Šupčić** – [ArkZeroRP](https://arkzerorp.com/) - [@SamKO_ArkZero](https://twitter.com/SamKO_ArkZero) - [@SamirSupcic](https://twitter.com/SamirSupcic)

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Contributing

1. Fork it (<https://github.com/SamKO91/ArkZeroRP_SamJSON>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

## Acknowledgments

* Hat tip to the good people at the ARK and ATLAS Modding Community
* **@Ghazlawl** (ARK and ATLAS Modding Community) for testing and providing good feedback

