# Awesome Qt  [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of awesome tools, libraries, and resources for the Qt framework.

-

## Contents

- TBD

## Official Resources

- Website

### Documentation

- Documentation

### Community

- Wiki

### Tools

A good developer writes his or her own tools.  A great one uses tools others wrote.  This section will help you be great; more formally, this section details applications that make it easier to create software with Qt.  You may also be interested in the [Libraries](#libraries) section.

## Official Tools

The Qt framework has surprisingly many tools that don't get the spotlight.  This section describes them (as well as the star players that do).

- [Qt Creator](https://www.qt.io/ide/) - By no means does Qt lock you into its provided IDE, but its firm integration with the framework makes it a good sell.  Among other things, it provides a UI designer, modeling tools, a documentation browser, and great QML support if you're into that sort of thing.  There's also a plugin system, but third-party plugins are unfortunately scarce.
  - [Qt Designer](http://doc.qt.io/qt-5/qtdesigner-manual.html) - If you'd rather just design the interfaces and let someone else hook them up to logic, the GUI designer is available as a separate application.
  - [Qt Assistant](http://doc.qt.io/qt-5/qtassistant-index.html) - So is the documentation viewer, for that matter.
- [Qt Visual Studio Add-in](http://doc.qt.io/vs-addin/index.html) - If you'd rather stick to Visual Studio, this add-in will let you do that.
- [Qt Linguist](http://doc.qt.io/qt-5/qtlinguist-index.html) - Qt provides excellent internationalization/localization support, and this tool is very much responsible for it.  Write translatable strings in your code with special macros, and this tool will aggregate them all for you so you or your translator(s) can broaden your software's audience.
- [Qt Installer Framework](http://doc.qt.io/qtinstallerframework/index.html) - Nobody seems to talk about this, but Qt also provides a way to write an installer for your application.  Does not support creation of OS X disk images or Linux packages, so be mindful of that when considering your project's distribution.
- [qmake](http://doc.qt.io/qt-5/qmake-manual.html) - A build system designed for Qt, though it can be used for non-Qt projects.
- [qbs](http://doc.qt.io/qbs/index.html) - If QML is more your style, this alternative build system might be up your alley.
- [Emulator](http://doc.qt.io/emulator/index.html) - Don't forget about Qt's mobile support!
- `qtdiag` - A command-line tool that prints out a lot of information pertaining to both your Qt installation and your system in general.  No link because there's no dedicated web page; just run `qtdiag` on the command line.  Excellent for troubleshooting.
- `qmleasing` - A curiously undocumented tool that lets you make easing curves suitable for QML, though if you understand the underlying math there's no reason you couldn't use the resulting numbers elsewhere.

## Third-Party Tools

- [CMake](http://doc.qt.io/qt-5/cmake-manual.html) - A general C++ build tool that happens to have great Qt support.
- [GammaRay](https://www.kdab.com/development-resources/qt-tools/gammaray/) - Powerful debugger and general inspection tool for Qt-built software.  Lets you inspect and manipulate the `QObject` hierarchy, view object properties, edit widgets at runtime, and far, *far* more.  A two-sentence blurb can't do it justice, seriously check it out.
- [SIP](https://www.riverbankcomputing.com/software/sip/intro) - Generates Python bindings for C or C++ libraries.  Has special support for Qt signals and slots, and was used to create [PyQt](https://riverbankcomputing.com/software/pyqt/intro).

## Bindings in Other Languages

- [Python (via PyQt)](https://riverbankcomputing.com/software/pyqt/intro) - Arguably the most comprehensive and well-known binding of Qt to another language.

...To be honest, that's the only one really worth mentioning as of this writing.  If you use a language that compiles to (or can easily and rapidly interface with) C++, I guess you could make something work.  If you're really so inclined, [these](http://www.ics.com/blog/using-qt-alternative-programming-languages-part-1) [two](http://www.ics.com/blog/using-qt-alternative-programming-languages-part-2) articles may pique your interest.

## Libraries

This section describes two kinds of third-party libraries; those that provide their own brand-new functionality (e.g. widgets), and those that provide integrations with existing software (e.g. scripting languages, clients for REST APIs).


### Integrations

- [QScintilla](https://riverbankcomputing.com/software/qscintilla/intro) - An absurdly versatile and customizable text editor widget that provides syntax highlighting, code completion, code folding, recordable macros, and *much* more.  Created by the same company that developed PyQt.

### New Functionality

- V-Play
- Qtilities
- KDE libraries

## Software Repositories

If the [Libraries](#libraries) section doesn't satisfy you, perhaps one of these will.

- [#inqlude](https://inqlude.org) - The most well-known aggregation of Qt-centric libraries out there.  A package manager is also available [here](https://inqlude.org/get.html).
- [QtPods](http://www.qt-pods.org) - Another Qt-centric package manager.  If you want to see the offerings without using QtPods, the full list is available [here](https://github.com/qt-pods/qt-pods-master/blob/master/pods.json), and can be added to by submitting a pull request.
- [Linux-Apps.com](https://www.linux-apps.com) - Despite the name, Linux-Apps.com aggregates a wide variety of Qt-based tools and libraries for both end-users and developers.
- [Stephan Binner's Ubuntu PPAs](https://launchpad.net/~beineri) - Ubuntu users who are hesitant to install anything outside of their package managers can obtain any recent version of Qt from these repositories.  Instructions for adding them are found within.

## Blogs

- [ICS](http://www.ics.com/blog) - A Qt-centric software consulting firm with a really neat blog.
- [Woboq](https://woboq.com/blog) - Another software consulting firm that also contributes code to Qt.
- KDAB
planet qt

## Tutorials

## Software that Uses Qt

A framework is only as great as the software that uses it.  Fortunately, much great software uses Qt.

- [Autodesk Maya](http://www.autodesk.com/maya) - 3D animation and design software that has been used to create visual effects for some of the most popular movies and TV shows of all time.
- [CMake](https://cmake.org) - The closest thing to a standard C++ build system out there. The bundled GUI uses Qt.
- [CRYENGINE](https://www.cryengine.com) - But can it run Crysis?
- [Doxygen](http://www.stack.nl/~dimitri/doxygen) - The most popular documentation generator for C++, though it supports other languages as well.  The bundled GUI uses Qt.
- [Google Earth](https://www.google.com/earth) - *The* virtual globe.
- [KDE](https://www.kde.org) - A popular desktop environment for Linux.
- [Parallels Desktop](http://www.parallels.com/products/desktop) - Consumer-focused virtualization.
- [Qt Creator](https://www.qt.io/ide) - Something something eating your own dog food. Listed in the [official resources](#official-resources), but not listing it here doesn't feel right.
- [RUBE](https://www.iforce2d.net/rube) - A level design tool for any game that uses the Box2D physics engine.
- [Skype](https://www.skype.com/en/download-skype/skype-for-linux) - Yes, *that* Skype.  Only the Linux version uses Qt.
- [TeamSpeak](http://www.teamspeak.com) - When gamers want to voice chat in a game that doesn't support it, they'll use this.
- [Tiled](http://www.mapeditor.org) - Perhaps the world's most popular tilemap editor.  Suitable for level design in games.
- [VirtualBox](https://www.virtualbox.org) - Virtualization software for x86/64 processors.  The bundled GUI uses Qt.
- [Wolfram Mathematica](http://www.wolfram.com/mathematica) - Programming language, symbolic calculator, and engineer's best friend.
- [Yabause](https://yabause.org) - A Sega Saturn emulator.
