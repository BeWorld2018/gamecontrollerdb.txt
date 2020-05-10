# GameControllerDB MORPHOS

A MorphOS community sourced database of game controller mappings to be used with SDL2 Game Controller functionality.

# Usage
Download gamecontrollerdb.txt, place it in your app's directory and load it.
You can put in ENVARC an reboot MorphOS to use one only file for all apps.

For example :
```
SDL_GameControllerAddMappingsFromFile("gamecontrollerdb.txt");
```

The database is compatible with SDL v2.0.10 and newer. Older SDL versions are no longer supported.

## Create New Mappings
A mapping looks like this :
```
030000004c050000cc09000000000000,PlayStation 4 Dualshock Controller,platform:MorphOS,a:b6,b:b7,x:b4,y:b5,back:b3,start:b2,leftstick:b8,rightstick:b9,leftshoulder:b0,rightshoulder:b1,dpup:h0.1,dpdown:h0.4,dpleft:h0.8,dpright:h0.2,leftx:a0,lefty:a1,rightx:a2,righty:a3,lefttrigger:+a4,righttrigger:+a5,
```
It is comprised of a controller GUID (`030000004c050000cc09000000000000`), a name (`PlayStation 4 Dualshock`), button / axis mappings (`leftshoulder:b0`) and a platform (`platform:MorphOS).

## Mapping Tools
There are a only one tool available now that let you create mappings.

### [SDL2 ControllerMap](https://www.morphos-storage.net/?page=Development%2FLibrary&file=SDL2_Libraries.lha)
The controllermap utility provided with SDL2 archive is the official tool to create these mappings.

## Resources

* [SDL2](http://www.libsdl.org)
* [SDL_GameControllerAddMappingsFromFile](http://wiki.libsdl.org/SDL_GameControllerAddMappingsFromFile)
