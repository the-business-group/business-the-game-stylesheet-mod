# Modding business-the-game (working title)
1. Make a fork of this represetory.
	- Optional: Rename .css-file to what sutes your project, and/or create new .css-files.
2. Do what you want.
3. Update the style header.
4. Push!

## Style header
The style header begins with `/**` and end with `**/` wrapped around a JSON.

|Field|Description|
|-|-|
|name|Name that will be displayed inside business-the-game.<br>Default: `""`|
|description|Plaintext description.<br>Default: `""`|
|imageUrl|URL or local path to image to be displayed togehter with Name.<br>Default: `""`|
|public|Set sheet for public listing (should this stylesheet be findable by others inside business-the-game?). If set to `false`, the sheet will still be usable, just harder to find.<br>Example: If the sheet is still under development or, is _this_ sheet just base sheet used by other sheets and should not be used by its own, set to `false`.<br>Default: `false`|
|using|Array with either a `string` path to file, or an object that reffer to an other stylesheet here on GitHub. This will be displayed to the user as recommended inclusions.<br>Default: `[]`|

Example:
```JSON
/**
{
	"name": "example",
	"description": "",
	"imageUrl": "",
	"public": false,
	"using": [
		"localRepresetoryFile.css",
		{
			"user": "testo",
			"repository": "business-the-game-stylesheet-mod-example",
			"file": "Classic.css"
		}
	]
}
**/
```