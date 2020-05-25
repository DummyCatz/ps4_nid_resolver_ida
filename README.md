# PS4 NID to Function Name Resolver
Resolves PS4 Bin/Lib Function Names

## Requirement
- IDA (Have only been tested on IDA 7.0)
- IDA SDK
- cmake
- [ps4libdoc](https://github.com/idc/ps4libdoc) by [@idc](https://github.com/idc)

## How-To-Build
```bash
git clone --recurse-submodules https://github.com/Thunder07/ps4_nid_resolver_ida.git
cd ps4_nid_resolver_ida
./extern/ida-cmake/build.py -t 7.0 -i ~/idasdk70/ --idaq ~/.idapro/
```
Note: on windows you'd need to change `--idaq C:\Users\USERNAME\AppData\Hex-Rays\IDA Pro\`

## How-To-Build Using Visual Studio 2017

1. Clone the repository

```bash
git clone --recurse-submodules https://github.com/DummyCatz/ps4_nid_resolver_ida.git
cd ps4_nid_resolver_ida
```

2. Copy your IDAPro7.0 SDK into ps4_nid_resolver_ida\idasdk70
3. The visual studio solution is in msvc folder

## How-To-Use

`Ctrl+Alt+F10`: Basic Settings Panel

`Ctrl+F10`: Resolve Function Names (Note: this action is none reversible, make sure you've a copy of your ida database before applying this)

## Special Thanks
To [@idc](https://github.com/idc) for his work on [ps4libdoc](https://github.com/idc/ps4libdoc) and [ps4-uplift](https://github.com/idc/ps4-uplift) which made this project possible.
