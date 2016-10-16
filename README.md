# Awesome Qt  [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of awesome tools, libraries, and resources for the Qt framework.

## Conventions

Any list item with an OctoCat :octocat: has a GitHub repo; click on it to see the source code!

## Contents

- TBD

## Official Resources

- [Official Website](https://www.qt.io/) - The official website for the Qt framework.
- [Qt Documentation](https://doc.qt.io/) - Official Qt documentation.  Massive and comprehensive.
- [Qt Bug Tracker](https://bugreports.qt.io/) - If you think you've found a bug with Qt or one of its related projects, report it here (or see if someone else already has).
- [Qt Code Review](https://codereview.qt-project.org) - See how the Qt maintainers ensure their code is well-written.
- [Source Code](https://code.qt.io/cgit/) [:octocat:](https://github.com/qt)/[:octocat:](https://github.com/qtproject) - Browse the various source trees that comprise the Qt project.

## Communities

If you build it, they will come.  This section describes aggregations of Qt users who share knowledge and code with one another.  The most popular and active communities are listed in this section, but you can find a more comprehensive list [here](https://wiki.qt.io/Online_Communities) (that includes several in other languages) if you'd prefer.

### Official

- [Qt Forum](https://forum.qt.io/) - If e-mail's not your thing, then you might also consider getting help or sharing knowledge on the forums.
- [Qt Wiki](https://wiki.qt.io/) - The premier source for user-contributed Qt knowledge.
- [Mailing Lists](http://lists.qt-project.org) - Mailing lists for users and developers of Qt alike.  Arguably the best place to communicate directly with Qt's maintainers.  Sees frequent activity.
- [IRC](https://webchat.freenode.net/?channels=%23qt%2C%23qt-quick%2C%23qt-creator%2C%23qt-chat) - For real-time chat with other Qt developers and users.  The most popular channels are on Freenode, and include `#qt`, `#qt-quick`, `#qt-creator`, and `#qt-chat`.
  - For a full list of Qt-related IRC channels, see [here](https://wiki.qt.io/Online_Communities#IRC_channels).
  - Note that the linked webchat client is *not* a part of the Qt project, and is made available by the author of this list for convenience only.  If there's another IRC client you'd prefer to use, go right ahead.

### Unofficial

- [QtForum.org](http://www.qtforum.org/) - Not to be confused with the official [Qt forum](https://forum.qt.io/).


## Tools

A good developer writes his or her own tools.  A great one uses tools others wrote.  This section will help you be great; more formally, this section details applications that make it easier to create software with Qt.  You may also be interested in the [Libraries](#libraries) section.

### Official Tools

The Qt framework has surprisingly many tools that don't get the spotlight.  This section describes them (as well as the star players that do).

- [Qt Creator](https://www.qt.io/ide/) [:octocat:](https://github.com/qtproject/qt-creator) - By no means does Qt lock you into its provided IDE, but its firm integration with the framework makes it a good sell.  Among other things, it provides a UI designer, modeling tools, a documentation browser, and great QML support if you're into that sort of thing.  There's also a plugin system, but third-party plugins are unfortunately scarce.
  - [Qt Designer](https://doc.qt.io/qt-5/qtdesigner-manual.html) [:octocat:](https://github.com/qt/qttools/tree/dev/src/designer) - If you'd rather just design the interfaces and let someone else hook them up to logic, the GUI designer is available as a separate application.
  - [Qt Assistant](https://doc.qt.io/qt-5/qtassistant-index.html) [:octocat:](https://github.com/qt/qttools/tree/dev/src/assistant) - So is the documentation viewer, for that matter.
- [Qt Visual Studio Add-in](https://doc.qt.io/vs-addin/index.html) - If you'd rather stick to Visual Studio, this add-in will let you do that.
- [Qt Linguist](https://doc.qt.io/qt-5/qtlinguist-index.html) [:octocat:](https://github.com/qt/qttools/tree/dev/src/linguist) - Qt provides excellent internationalization/localization support, and this tool is very much responsible for it.  Write translatable strings in your code with special macros, and this tool will aggregate them all for you so you or your translator(s) can broaden your software's audience.
- [Qt Installer Framework](https://doc.qt.io/qtinstallerframework/index.html) [:octocat:](https://github.com/qtproject/installer-framework) - Nobody seems to talk about this, but Qt also provides a way to write an installer for your application.  Does not support creation of macOS disk images, app bundles, or Linux packages, so be mindful of that when considering your project's distribution.
  - [`macdeployqt`](https://doc.qt.io/qt-5/osx-deployment.html) [:octocat:](https://github.com/qt/qttools/tree/dev/src/macdeployqt) - A tool for generating macOS application bundles for Qt projects.
- [qmake](https://doc.qt.io/qt-5/qmake-manual.html) - A build system designed for Qt, though it can be used for non-Qt projects.
- [qbs](https://doc.qt.io/qbs/index.html) - If QML is more your style, this alternative build system might be up your alley.
- [Emulator](https://doc.qt.io/emulator/index.html) - Don't forget about Qt's mobile support!
- `qtdiag` [:octocat:](https://github.com/qt/qttools/tree/dev/src/qtdiag) - A command-line tool that prints out a lot of information pertaining to both your Qt installation and your system in general.  No link because there's no dedicated web page; just run `qtdiag` on the command line.  Excellent for troubleshooting.
- `qmleasing` - A curiously undocumented tool that lets you make easing curves suitable for QML, though if you understand the underlying math there's no reason you couldn't use the resulting numbers elsewhere.

### Third-Party Tools

- [CMake](https://doc.qt.io/qt-5/cmake-manual.html) [:octocat:](https://github.com/Kitware/CMake) - A general C++ build tool that happens to have great Qt support.
- [GammaRay](https://www.kdab.com/development-resources/qt-tools/gammaray/) [:octocat:](https://github.com/KDAB/GammaRay) - Powerful debugger and general inspection tool for Qt-built software.  Lets you inspect and manipulate the `QObject` hierarchy, view object properties, edit widgets at runtime, and far, *far* more.  A two-sentence blurb can't do it justice, seriously check it out.
- [SIP](https://www.riverbankcomputing.com/software/sip/intro) - Generates Python bindings for C or C++ libraries.  Has special support for Qt signals and slots, and was used to create [PyQt](https://riverbankcomputing.com/software/pyqt/intro).

## Bindings in Other Languages

- [Python (via PyQt)](https://riverbankcomputing.com/software/pyqt/intro) - Arguably the most comprehensive and well-known binding of Qt to another language.
- [Python (via PySide)](https://github.com/PySide) - Another binding for Python, which has been officially adopted by the Qt project.
- [Ring (via RingQt)](http://ring-lang.sourceforge.net/doc/qt.html) -

See these [these](https://www.ics.com/blog/using-qt-alternative-programming-languages-part-1) [three](https://www.ics.com/blog/using-qt-alternative-programming-languages-part-2) [articles](https://wiki.qt.io/Category:LanguageBindings) if you want more.

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

- [Planet Qt](https://planet.qt.io/) - Official aggregation of Qt-related blogs.
- [ICS](https://www.ics.com/blog) - A Qt-centric software consulting firm with a really neat blog.
- [Woboq](https://woboq.com/blog) - Another software consulting firm that also contributes code to Qt.
- [KDAB](https://www.kdab.com/category/blogs/) - *Another* consulting firm that specializes in Qt.

## Tutorials

## Software that Uses Qt

A framework is only as great as the software that uses it.  Fortunately, much great software uses Qt.

- [Autodesk Maya](http://www.autodesk.com/maya) - 3D animation and design software that has been used to create visual effects for some of the most popular movies and TV shows of all time.
- [CMake](https://cmake.org) [:octocat:](https://github.com/Kitware/CMake) - The closest thing to a standard C++ build system out there. The bundled GUI uses Qt.
- [CRYENGINE](https://www.cryengine.com) [:octocat:](https://github.com/CRYTEK-CRYENGINE/CRYENGINE) - But can it run Crysis?
- [Doxygen](https://www.stack.nl/~dimitri/doxygen) [:octocat:](https://github.com/doxygen/doxygen) - The most popular documentation generator for C++, though it supports other languages as well.  The bundled GUI uses Qt.
- [Google Earth](https://www.google.com/earth) - *The* virtual globe.
- [KDE](https://www.kde.org) [:octocat:](https://github.com/KDE) - A popular desktop environment for Linux.
- [Parallels Desktop](http://www.parallels.com/products/desktop) - Consumer-focused virtualization.
- [Qt Creator](https://www.qt.io/ide) [:octocat:](https://github.com/qtproject/qt-creator) - Something something eating your own dog food. Listed in the [official tools](#official-tools), but not listing it here doesn't feel right.
- [RUBE](https://www.iforce2d.net/rube) - A level design tool for any game that uses the Box2D physics engine.
- [Skype](https://www.skype.com/en/download-skype/skype-for-linux) - Yes, *that* Skype.  Only the Linux version uses Qt.
- [TeamSpeak](http://www.teamspeak.com) - When gamers want to voice chat in a game that doesn't support it, they'll use this.
- [Tiled](http://www.mapeditor.org) [:octocat:](https://github.com/bjorn/tiled) - Perhaps the world's most popular tilemap editor.  Suitable for level design in games.
- [VirtualBox](https://www.virtualbox.org) - Virtualization software for x86/64 processors.  The bundled GUI uses Qt.
- [Wolfram Mathematica](https://www.wolfram.com/mathematica) - Programming language, symbolic calculator, and engineer's best friend.
- [Yabause](https://yabause.org) [:octocat:](https://github.com/Yabause/yabause) - A Sega Saturn emulator.

There's also an official showroom [here](https://showroom.qt.io/), which lets developers submit their own Qt-powered applications for display.
