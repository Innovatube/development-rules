# iOS Development Guidelines

## Language

Use Swift ( Latest version ). Never use Objective-C anymore.

## Package Manager

Use CocoaPods and specify minor version ( x.x ) at least on Podfile. Never add any third-party libraries without using CocoaPods.

And use libraries only written in Swift. Never use libraries which is written in Objective-C. Use XXX to find libraries which is written in Swift.

If there is any special SDKs which surely required from the Client, you can add it without using CocoaPods.

## Directory Structure

Sync project structure with file/directory structure. Use [synx](https://github.com/venmo/synx) to sync them.

## Support iOS Versions

Default support version of iOS is Latest + previous versions. If latest version is iOS9, need to support iOS8 and iOS9.

But if client requires to support older versions and project manager accepted it, you need to follow.

## StoryBoards

If you use storyboards, you never build one huge monolithic storyboard file. You need to split storyboard to multiple files.

## Use Vector file and Fonts for images

You need to use vector (SVG) / font files for icons, logos, and any other mono color pixel art images. You can use raster images ( jpeg, png.. ) only for photo and full color images.



