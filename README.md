# SamJSON
> UnrealEngine Graphs based JSON Library

SamJSON is a JSON Library that was created to be used by Modders of UnrealEngine based games like ARK and ATLAS where there is no access to the source code and all functionalities need to be implemented using the Blueprints Graphs System.

![](Screenshot_0.png)

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

* /ArkZeroRP/SamJSON/SamJSON.uasset - [#f03c15]REQUIRED
_The library BP based of Object_
* /ArkZeroRP/SamJSON/SamJSON_ExampleSingleton.uasset - [#1589F0]OPTIONAL
_Examples singleton BP based of Actor_
* /ArkZeroRP/SamJSON/Enums/SamJSON_DataType.uasset - [#f03c15]REQUIRED
_Enum BP, possible types of Properties or Array Items_
* /ArkZeroRP/SamJSON/Enums/SamJSON_ValueErrorType.uasset - [#f03c15]REQUIRED
_Enum BP, possible types of Errors when using GetPropertyAsX_
* /ArkZeroRP/SamJSON/Structs/SamJSON_KeyValue.uasset - [#f03c15]REQUIRED
_Struct BP, represents a single property as Key/Value/Type_
* /ArkZeroRP/SamJSON/Structs/Z_BoolMap.uasset - [#f03c15]REQUIRED
_Struct BP, represents a property as Key(String)/Value(Boolean) - Used for bulk adding of properties to a SamJSON object_
* /ArkZeroRP/SamJSON/Structs/Z_NumberMap.uasset - [#f03c15]REQUIRED
_Struct BP, represents a property as Key(String)/Value(Float) - Used for bulk adding of properties to a SamJSON object_
* /ArkZeroRP/SamJSON/Structs/Z_StringMap.uasset - [#f03c15]REQUIRED
_Struct BP, represents a property as Key(String)/Value(String) - Used for bulk adding of properties to a SamJSON object_

### Usage example

* Open "SamJSON_ExampleSingleton" to see examples of how to use the "SamJSON" Blueprint that is the JSON Library itself
* (ARK/ATLAS)You can add "SamJSON_ExampleSingleton" to your singletons list in the PrimalGameData to execute it in PIE and see the examples in action

![](Screenshot_1.png)

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

[https://github.com/yourname/github-link](https://github.com/dbader/)

## Contributing

1. Fork it (<https://github.com/SamKO91/ArkZeroRP_SamJSON>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

## Acknowledgments

* Hat tip to the good people at the ARK and ATLAS Modding Community
* **@Ghazlawl** (ARK and ATLAS Modding Community) for testing and providing good feedback

