# Using Third Party Libraries

## Package Manager

You must use package managers.

| Language | PackageManager |
|:---------|:---------------|
| PHP      | Composer       |
| Ruby     | Gem            |
| Python   | pip            |
| Swift    | CocoaPods      |
| Java     | Gradle         |

You must not use any third party library which is not registered to package manager registory.

## Version Management

You must specify at least minor version "x.x" when you use thirdparty libraries. Should not speciy only "major" version.
Should not use "development" version or "alpha" version.

## Old Libraries

You should not use too old libraries. If the library has not updated more than 1 year, never use it. You must find newer libraries.


