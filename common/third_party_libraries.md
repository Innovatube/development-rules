# Using Third Party Libraries

## Package Manager

You must use package managers.

| Language | PackageManager    |
|:---------|:------------------|
| PHP      | Composer          |
| Ruby     | Gem               |
| Python   | pip               |
| Swift    | CocoaPods/carthage|
| Java     | Gradle            |

You must not use any third party library which is not registered to package manager registry.

It's for ensuring every developers can use same version of library.

## Version Management

You must specify at least minor version "x.x" when you use third party libraries. Should not specify only "major" version.
Should not use "development" version or "alpha" version.

Because if you don't fix the version, app may stop working when the library introduces braking changes.

## Old Libraries

You should not use too old libraries. If the library has not updated more than 1 year, never use it. You must find newer libraries.

## License

You need to check third party library license especially you need to bundle it to the app binary ( using in client applications ). You can only use the libraries distributed with the following licenses.

* MIT License
* Apache License
* Do What the Fuck You Want to Public License

Never use GPL/LGPL and other licenses.

## Isn't it too huge ?

The library's core function is the function which you need to use in the app? If you want to use library for using it's "sub" feature, you may not use it and try to find alternatives ( or implement by your self )

## Summary: You never use the following libraries

* Doesn't registered to Package Manager Repository
* Doesn't follow semantic versioning
* Has not updated for more than 1 year
* Need to use "sub" feature only in the library