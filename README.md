# Build Version Widget Library

This package serves a widget library to be paired with the [BuildVersion](https://github.com/br-na-pm/BuildVersion#readme) PowerShell script package.  
BuildVersion is a software package for Automation Studio to automatically collect version information from a git repository.  
This widget library provides single binding widgets to quickly display a range of git version information.  

**NOTE:** This is not an official package and is provided as-in under the GPL v3.0 license.

## Features

- Single structure binding
	- Users can simply use the existing structure defined in [BuildVersion](https://github.com/br-na-pm/BuildVersion#readme)
- Multiple compound widgets
	- Basic
	- Standard
	- Advanced
- Change warning indicator
	- Notify users when uncommitted changes are detected

## Widgets

### Basic

### Standard

### Advanced

## Binding

A single binding is required to populate the widgets with build information.

```xml
<Binding mode="oneWay">
  <Source xsi:type="opcUaComplexObject" refId="::BuildVer:BuildVersion" />
  <Target xsi:type="brease" contentRefId="content_0" widgetRefId="BuildVersionStandard1" attribute="value" />
</Binding>
```
