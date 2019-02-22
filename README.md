# Awesome Qt  [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

[<img src="https://cdn.rawgit.com/JesseTG/awesome-qt/ef9f71a9/qt.svg" align="right" width="100">](https://www.qt.io)

> A curated list of awesome tools, libraries, and resources for the Qt framework.

[Qt](https://www.qt.io) is a powerful cross-platform application development framework, for use primarily (but not exclusively) in C++.  It's great for GUI applications, but can be used for many other things as well.

Contributions are welcome!

## Conventions

- Any list item with an OctoCat :octocat: has a GitHub repo or organization; click on it to see the source code!
- List items with this :package: icon have source code hosted elsewhere.

## Contents

- [Official Resources](#official-resources)
- [Communities](#communities)
  - [Official](#official)
  - [Unofficial](#unofficial)
- [Tools](#tools)
  - [Official Tools](#official-tools)
  - [Third-Party Tools](#third-party-tools)
- [Bindings in Other Languages](#bindings-in-other-languages)
- [Libraries](#libraries)
  - [Integrations](#integrations)
  - [New Functionality](#new-functionality)
- [Software Repositories](#software-repositories)
- [Blogs](#blogs)
- [Books](#books)
- [Software that Uses Qt](#software-that-uses-qt)
- [Other Relevant Awesome Lists](#other-relevant-awesome-lists)
- [License](#license)

## Official Resources

- [Official Website](https://www.qt.io) - The official website for the Qt framework.
- [Qt Documentation](https://doc.qt.io) - Official Qt documentation.  Massive and comprehensive.
- [Qt Newsletters](https://www.qt.io/newsletters) - The best of Qt, straight to your spam filter.
- [Qt Bug Tracker](https://bugreports.qt.io) - If you think you've found a bug with Qt or one of its related projects, report it here (or see if someone else already has).
- [Qt Code Review](https://codereview.qt-project.org) - See how the Qt maintainers ensure their code is well-written.
- [Source Code](https://code.qt.io) - Browse the various source trees that comprise the Qt project.  Has mirrors at several GitHub organizations:
  - Qt [:octocat:](https://github.com/qt)
  - Qt Project [:octocat:](https://github.com/qtproject)
  - Qt Labs [:octocat:](https://github.com/qt-labs)

## Communities

If you build it, they will come.  This section describes aggregations of Qt users who share knowledge and code with one another.  The most popular and active communities are listed in this section, but you can find a more comprehensive list [here](https://wiki.qt.io/Online_Communities) (that includes several in other languages) if you'd prefer.

### Official

- [Mailing Lists](http://lists.qt-project.org) - Mailing lists for users and developers of Qt alike.  Arguably the best place to communicate directly with Qt's maintainers.  Sees frequent activity.
- [Qt Forum](https://forum.qt.io) - If e-mail's not your thing, then you might also consider getting help or sharing knowledge on the forums.
- [Qt Wiki](https://wiki.qt.io) - The premier source for user-contributed Qt knowledge.
- [IRC](https://webchat.freenode.net/?channels=%23qt%2C%23qt-quick%2C%23qt-creator%2C%23qt-chat) - For real-time chat with other Qt developers and users.  The most popular channels are on Freenode, and include `#qt`, `#qt-quick`, `#qt-creator`, and `#qt-chat`.
  - For a full list of Qt-related IRC channels, see [here](https://wiki.qt.io/Online_Communities#IRC_channels).
  - Note that the linked webchat client is *not* a part of the Qt project, and is provided by the author of this list for convenience only.  These channels can be accessed through any IRC client.

### Unofficial

- [QtForum.org](http://www.qtforum.org) - Not to be confused with the official [Qt forum](https://forum.qt.io).


## Tools

A good developer writes his or her own tools.  A great one uses tools others wrote.  This section will help you be great; more formally, this section details applications that make it easier to create software with Qt.  You may also be interested in the [Libraries](#libraries) section.

### Official Tools

The Qt framework has surprisingly many tools that don't get the spotlight.  This section describes them (as well as the star players that do).  For the purpose of this section, "tool" refers to Qt-centric utilities whose code does *not* get embedded within your application (but their output might).

- [Qt Creator](https://www.qt.io/ide) [:octocat:](https://github.com/qtproject/qt-creator) - By no means does Qt lock you into its provided IDE, but its firm integration with the framework makes it a good sell.  Among other things, it provides a UI designer, modeling tools, a documentation browser, and great QML support if you're into that sort of thing.  There's also a plugin system, but third-party plugins are unfortunately scarce.
  - [Qt Designer](https://doc.qt.io/qt-5/qtdesigner-manual.html) [:octocat:](https://github.com/qt/qttools/tree/dev/src/designer) - If you'd rather just design the interfaces and let someone else hook them up to logic, the GUI designer is available as a separate application.
  - [Qt Assistant](https://doc.qt.io/qt-5/qtassistant-index.html) [:octocat:](https://github.com/qt/qttools/tree/dev/src/assistant) - So is the documentation viewer, for that matter.
- [Qt Visual Studio Add-in](https://doc.qt.io/archives/vs-addin) [:octocat:](https://github.com/qt-labs/vstools) - If you'd rather stick to Visual Studio, this add-in will let you do that.
- [Qt Linguist](https://doc.qt.io/qt-5/qtlinguist-index.html) [:octocat:](https://github.com/qt/qttools/tree/dev/src/linguist) - Qt provides excellent internationalization/localization support, and this tool is very much responsible for it.  Write translatable strings in your code with special macros, and this tool will aggregate them all for you so you or your translator(s) can broaden your software's audience.
- [Qt Installer Framework](https://doc.qt.io/qtinstallerframework) [:octocat:](https://github.com/qtproject/installer-framework) - Nobody seems to talk about this, but Qt also provides a way to write an installer for your application.  Does not support creation of macOS disk images, app bundles, or Linux packages, so be mindful of that when considering your project's distribution.
  - [`macdeployqt`](https://doc.qt.io/qt-5/osx-deployment.html) [:octocat:](https://github.com/qt/qttools/tree/dev/src/macdeployqt) - Generates macOS application bundles for Qt projects.
- [qmake](https://doc.qt.io/qt-5/qmake-manual.html) [:octocat:](https://github.com/qt/qtbase/tree/dev/qmake) - The bundled build system designed for Qt, though it can be used for non-Qt projects.
- [qbs](https://doc.qt.io/qbs) [:octocat:](https://github.com/qt-labs/qbs) - If QML is more your style, consider this alternative build system.
- [Emulator](https://doc.qt.io/emulator) - Don't forget about Qt's mobile support!
- `qtdiag` [:octocat:](https://github.com/qt/qttools/tree/dev/src/qtdiag) - Command-line tool that prints out a lot of information pertaining to both your Qt installation and your system in general.  No link because there's no dedicated web page; just run `qtdiag` on the command line.  Excellent for troubleshooting.
- `qmleasing` [:octocat:](https://github.com/qt/qtdeclarative/tree/dev/tools/qmleasing) - Lets you make easing curves suitable for QML, though if you understand the underlying math there's no reason you couldn't use the resulting numbers elsewhere.

### Third-Party Tools

- [CMake](https://doc.qt.io/qt-5/cmake-manual.html) [:octocat:](https://github.com/Kitware/CMake) - General C++ build tool that happens to have great Qt support.
- [GammaRay](https://www.kdab.com/development-resources/qt-tools/gammaray) [:octocat:](https://github.com/KDAB/GammaRay) - Powerful debugger and general inspection tool for Qt-built software.  Lets you inspect and manipulate the `QObject` hierarchy, view object properties, edit widgets at runtime, and far, *far* more.  A two-sentence blurb can't do it justice, seriously check it out.
- [moc-ng](https://github.com/woboq/moc-ng) [:octocat:](https://github.com/woboq/moc-ng) - Alternative implementation of `moc` that's binary-compatible with Qt's version.
- [Qt-Inspector](https://github.com/robertknight/Qt-Inspector) [:octocat:](https://github.com/robertknight/Qt-Inspector) - Inspection tool with similar goals to GammaRay, though much simpler.
- [SIP](https://www.riverbankcomputing.com/software/sip) [:package:](https://www.riverbankcomputing.com/hg/sip) - Generates Python bindings for C or C++ libraries.  Has special support for Qt signals and slots, and was used to create [PyQt](https://riverbankcomputing.com/software/pyqt).
- [linuxdeployqt](https://github.com/probonopd/linuxdeployqt) [:octocat:](https://github.com/probonopd/linuxdeployqt) - Lets you bundle your Qt based application as an AppDir or [AppImage](http://appimage.org), making it possible to ship it to users of many desktop Linux distributions. Similar to the official `windeployqt` and `macdeployqt` tools but for Linux.

## Bindings in Other Languages

This section describes software that enables creation of Qt software in a primary language other than C++.  Libraries that allow run-time scripting in a Qt application are listed under [Integrations](#integrations).

- [Python (via PyQt)](https://riverbankcomputing.com/software/pyqt) [:package:](https://www.riverbankcomputing.com/software/pyqt/download5) - Arguably the most comprehensive and well-known binding of Qt to another language.
- [Python (via PySide)](https://wiki.qt.io/PySide) [:package:](https://code.qt.io/cgit/pyside/pyside.git) - Another binding for Python, which has been officially adopted by the Qt project.
- [Ring (via RingQt)](http://ring-lang.sourceforge.net/doc/qt.html) [:octocat:](https://github.com/ring-lang/ring/tree/master/extensions/ringqt) - I've never heard of this language either, honestly.
- [Mono/.NET languages (via QtSharp)](https://github.com/ddobrev/QtSharp) [:octocat:](https://github.com/ddobrev/QtSharp) - Experimental wrapper for Qt that allows it to be used by .NET-based languages such as C#.  Young, but active.

See these [these](https://www.ics.com/blog/using-qt-alternative-programming-languages-part-1) [three](https://www.ics.com/blog/using-qt-alternative-programming-languages-part-2) [articles](https://wiki.qt.io/Category:LanguageBindings) if you want more.

## Libraries

This section describes two kinds of third-party libraries; those that provide their own brand-new functionality (e.g. widgets, dealing with particular file formats), and those that provide integrations with existing software (e.g. scripting languages, clients for REST APIs, implementations of established protocols).


### Integrations

For the purpose of this section, an "Integration"-focused library does one of the following:

1. Serves as a client for an established Web service.
2. Wraps another library in a Qt-friendly manner as more than just an implementation detail (i.e. it tries to mimic the wrapped API).


- [mupdf-qt](https://xiangxw.github.io/mupdf-qt) [:octocat:](https://github.com/xiangxw/mupdf-qt) - Qt wrapper for the [MuPDF](https://mupdf.com) PDF viewer.
- [neiasound](https://github.com/lucaspcamargo/neiasound) [:octocat:](https://github.com/lucaspcamargo/neiasound) - OpenAL wrapper designed for games, with [stb_vorbis](https://nothings.org/stb_vorbis) and [libsndfile](http://www.mega-nerd.com/libsndfile) support.
- [PythonQt](http://pythonqt.sourceforge.net) [:package:](https://sourceforge.net/projects/pythonqt) - Script your Qt applications with Python.  Not to be confused with [PyQt](https://riverbankcomputing.com/software/pyqt) or [PySide](https://wiki.qt.io/PySide).
- [QScintilla](https://riverbankcomputing.com/software/qscintilla) [:package:](https://www.riverbankcomputing.com/software/qscintilla/download) - Absurdly versatile and customizable text editor widget that provides syntax highlighting, code completion, code folding, recordable macros, and *much* more.  Built around [Scintilla](http://www.scintilla.org).  Created by the same company that developed [PyQt](https://riverbankcomputing.com/software/pyqt).
- [QtAwesome](https://github.com/gamecreature/QtAwesome) [:octocat:](https://github.com/gamecreature/QtAwesome) - Add [Font Awesome](https://fortawesome.github.io/Font-Awesome) icons to your Qt application.  Other icon sets are supported, too.
- [QtLua](http://www.nongnu.org/libqtlua) [:package:](https://svn.savannah.nongnu.org/viewvc/?root=libqtlua) - Use Lua as a scripting language for Qt-based software.
- [qtruby](https://github.com/cybercatalyst/qtruby) [:octocat:](https://github.com/cybercatalyst/qtruby) - Use Ruby as a scripting language within your application.
- [QuaZIP](http://quazip.sourceforge.net) [:package:](https://sourceforge.net/projects/quazip) - Read from and write to ZIP archives.  Uses [Minizip](http://www.winimage.com/zLibDll/minizip.html) under the hood.
- [VLC-Qt](https://vlc-qt.tano.si) [:octocat:](https://github.com/vlc-qt/vlc-qt) - Wrapper for [libvlc](https://wiki.videolan.org/LibVLC) that lets you add a VLC-like media player to your application.

### New Functionality

- [Communi](https://communi.github.io) [:octocat:](https://github.com/communi/libcommuni) - Cross-platform IRC framework.  We've got enough IRC clients out there already, but I suppose this could also be used to implement a chat function in your application (e.g. for community support).
- [cutelyst](http://cutelyst.org) [:octocat:](https://github.com/cutelyst/cutelyst) - Web framework that takes some ideas from Perl's Catalyst framework.
- [DiceParser](https://github.com/Rolisteam/DiceParser) [:octocat:](https://github.com/Rolisteam/DiceParser) - Dice Roller framework based on its own syntax. 
- [DOtherSide](https://github.com/filcuc/DOtherSide) [:octocat:](https://github.com/filcuc/DOtherSide) - Binding for QML in C, primarily designed as an API for *other* languages to support QML.
- [Felgo](https://felgo.com) - Cross-platform game engine and app framework that relies heavily on QML.  Has a lot of tools and resources, and may even deserve its own list.
- [glraw](https://github.com/cginternals/glraw) [:octocat:](https://github.com/cginternals/glraw) - Convert images from any Qt-supported format to OpenGL-format textures.  Useful for speeding up texture loading in graphics applications.
- [grantlee](https://github.com/steveire/grantlee) [:octocat:](https://github.com/steveire/grantlee) - Django-inspired text templating.
- [injeqt](https://github.com/vogel/injeqt) [:octocat:](https://github.com/vogel/injeqt) - Dependency injection for Qt.
- [KDE Frameworks](https://api.kde.org/frameworks) [:octocat:](https://github.com/KDE) [:package:](https://quickgit.kde.org) - Metric ass-ton of libraries for KDE, but many of them can be used with regular Qt applications as well.  Cross-platform, for the most part.
- [Marble](https://marble.kde.org) [:package:](https://cgit.kde.org/marble.git) - Virtual globe and map that can be used standalone or embedded within other applications.
- [qgexedit2](https://github.com/Simsys/qhexedit2) [:octocat:](https://github.com/Simsys/qhexedit2) - Embed a hex editor in your application.
- [qml-material](https://github.com/papyros/qml-material) [:octocat:](https://github.com/papyros/qml-material) - Material Design implemented in QML.
- [QNodeView](https://github.com/gwihlidal/QNodeView) [:octocat:](https://github.com/gwihlidal/QNodeView) - Widget that lets you create and edit nodes in a graph similar to the kind provided by Unreal Engine, Substance Designer, or PureData.
- [QSimpleUpdater](https://github.com/alex-spataru/QSimpleUpdater) [:octocat:](https://github.com/alex-spataru/QSimpleUpdater) - Let your application update itself.
- [qt-maybe](https://github.com/robertknight/qt-maybe) [:octocat:](https://github.com/robertknight/qt-maybe) - Fans of type theory will enjoy these sum and optional types.
- [qt-mustache](https://github.com/robertknight/qt-mustache) [:octocat:](https://github.com/robertknight/qt-mustache) - Render [Mustache](https://mustache.github.io) templates.
- [QtAV](http://www.qtav.org) [:octocat:](https://github.com/wang-bin/QtAV) - Actively developed multimedia framework.
- [Qtilities](https://jpnaude.github.io/Qtilities) [:octocat:](https://github.com/JPNaude/Qtilities) - Powerful set of libraries that provide GUI, logging, testing, configuration, and project functionality (among other things) for your application.
- [QtitanChart](http://www.devmachines.com/qtitanchart-overview) - Chart generation framework.  Commercial.
- [QtitanRibbon](http://www.devmachines.com/qtitanribbon-overview) - For fans of the ribbons that Microsoft uses in their software.  Commercial.
- [qtnotify](https://github.com/cybercatalyst/qtnotify) [:octocat:](https://github.com/cybercatalyst/qtnotify) - Notification framework.
- [QtTerminalWidget](https://github.com/cybercatalyst/qtterminalwidget) [:octocat:](https://github.com/cybercatalyst/qtterminalwidget) - Make your application capable of **anything**.
- [QtVerbalExpressions](https://github.com/VerbalExpressions/QtVerbalExpressions) [:octocat:](https://github.com/VerbalExpressions/QtVerbalExpressions) - Create regular expressions using natural English expressions.  Part of the [VerbalExpressions](https://verbalexpressions.github.io) project, which does the same thing for a wide variety of languages.
- [qtwebserver](https://github.com/cybercatalyst/qtwebserver) [:octocat:](https://github.com/cybercatalyst/qtwebserver) - If you need to write a web application server in Qt for some reason, this'll help you along.
- [QtXlsx](http://qtxlsx.debao.me) [:octocat:](https://github.com/dbzhang800/QtXlsxWriter) - Read and write spreadsheets in Microsoft Excel format.
- [Qwt](http://qwt.sourceforge.net) [:package:](https://sourceforge.net/projects/qwt) - Qt widgets designed for scientific and technical applications.
- [verdigris](https://github.com/woboq/verdigris) [:octocat:](https://github.com/woboq/verdigris) - Experimental library to write Qt applications *without* using the `moc`.

## Software Repositories

If the [Libraries](#libraries) section doesn't satisfy you, perhaps one of these will.

- [#inqlude](https://inqlude.org) - The most well-known aggregation of Qt-centric libraries out there.  A package manager is also available [here](https://inqlude.org/get.html).
- [QtPods](https://github.com/qt-pods/qt-pods) - Another Qt-centric package manager.  If you want to see the offerings without using QtPods, the full list is available [here](https://github.com/qt-pods/qt-pods-master/blob/master/pods.json), and can be added to by submitting a pull request.
- [Linux-Apps.com](https://www.linux-apps.com) - Despite the name, Linux-Apps.com aggregates a wide variety of Qt-based tools and libraries for both end-users and developers.
- [Stephan Binner's Ubuntu PPAs](https://launchpad.net/~beineri) - Ubuntu users who are hesitant to install anything outside of their package managers can obtain any recent version of Qt from these repositories.  Instructions for adding them are found within.

## Blogs

Each entry is followed by a standout list of articles, talks, or other resources.

- [Planet Qt](https://planet.qt.io) - Official aggregation of first-party and third-party Qt-related blogs.
- [ICS](https://www.ics.com/blog) - Qt-centric software consulting firm with a really neat blog.  Specializes in graphics applications.
  - Qt Tips and Tricks [[1](https://www.ics.com/blog/qt-tips-and-tricks-part-1), [2](https://www.ics.com/blog/qt-tips-and-tricks-part-2)] - Odds and ends that might be nice to keep in your back pocket.
  - [Mastering Qt File Selectors](https://www.ics.com/blog/mastering-qt-file-selectors) - Sometimes you need different variations of the same asset, but you won't know which ones to load until runtime.  This class will decide for you.
  - Some Lesser Known Qt Tools and Commands [[1](https://www.ics.com/blog/some-lesser-known-qt-tools-and-commands-part-1), [2](https://www.ics.com/blog/some-lesser-known-qt-tools-and-commands-part-2), [3](https://www.ics.com/blog/some-lesser-known-qt-tools-and-commands-part-3), [4](https://www.ics.com/blog/some-lesser-known-qt-tools-and-commands-part-4), [5](https://www.ics.com/blog/some-lesser-known-qt-tools-and-commands-part-5)] - You don't find hidden gems by staying on the beaten path.
  - [Using Self-Signed Certificates in Qt Code](https://www.ics.com/blog/using-self-signed-certificates-qt-code) - Trust nobody.
  - [Integrating C++ with QML](https://www.ics.com/blog/integrating-c-qml) - Talk to your scripting language.  That's what it's there for.
  - Qt and OpenGL: Loading a 3D Model with Open Asset Import Library (Assimp) [[1](https://www.ics.com/blog/qt-and-opengl-loading-3d-model-open-asset-import-library-assimp), [2](https://www.ics.com/blog/qt-and-opengl-loading-3d-model-open-asset-import-library-assimp-part-2)] - Assimp supports a lot of different model types; these articles will help you support all of them.
  - [What's new in Qt 5: QStandardPaths](https://www.ics.com/blog/whats-new-qt-5-qstandardpaths) - This feature's been around for a few years, but it's still useful enough to warrant an entry on this list.
  - [What's New in Qt 5.2: QCommandLineParser](https://www.ics.com/blog/whats-new-qt-52-qcommandlineparser) - Another oldie, but still a goodie.
- [Woboq](https://woboq.com/blog) - Another software consulting firm that also contributes code to Qt.  They seem to specialize in Qt's core architecture.
  - [Moc myths debunked](https://woboq.com/blog/moc-myths.html) - The magic that Qt appears to rely in is really just a bunch of code generators.  This post will bring you up to speed on the reality of the `moc`, the most notable one.
  - How Qt Signals and Slots Work [[1](https://woboq.com/blog/how-qt-signals-slots-work.html), [2](https://woboq.com/blog/how-qt-signals-slots-work-part2-qt5.html), [3](https://woboq.com/blog/how-qt-signals-slots-work-part3-queuedconnection.html)] - Qt's signals/slots system lets any object talk to any other object.  Understanding these three articles will help you take full advantage of the feature.
  - [QMetaType knows your types](https://woboq.com/blog/qmetatype-knows-your-types.html) - C++ isn't known for having good run-time type information, so Qt brings its own.
  - [C++11 in Qt5](https://woboq.com/blog/cpp11-in-qt5.html) - Stop writing C++ like it's 2003; learn how you can take advantage of recent C++ features in your Qt applications.
  - [C++14 for Qt programmers](https://woboq.com/blog/cpp14-in-qt.html) - `s/2003/2011/`
  - [QStringLiteral explained](https://woboq.com/blog/qstringliteral.html) - String literals are widely used in many applications; wouldn't it be nice if you could make them faster to access?
  - [Nicer debug output in Qt using QT_MESSAGE_PATTERN](https://woboq.com/blog/nice-debug-output-with-qt.html) - It's nice to be able to read your application's logs.
- [KDAB](https://www.kdab.com/category/blogs) - *Another* consulting firm that specializes in Qt.
  - [GammaRay: Taking a deep look into your Qt application](https://www.youtube.com/watch?v=JcoFk_PVhdk) - Talk about [GammaRay](https://www.kdab.com/development-resources/qt-tools/gammaray) and how it can help you dissect your Qt applications.  Talk given at QtCon 2016 by [Volker Krause](https://github.com/vkrause).
  - [Multithreading with Qt](https://www.youtube.com/watch?v=dcSsjxhazu0) - I want to make my application do more than once thing at once.  What could possibly go wrong?  Talk given at QtCon 2016 by [Giuseppe D'Angelo](https://github.com/dangelog).
  - [Linux perf for Qt developers](https://www.youtube.com/watch?v=L4NClVxqdMw) - How to make your Qt application faster, Linux-style.  Talk given at QtCon 2016 by [Milian Wolff](https://github.com/milianw).

## Books

- [Qt5 C++ GUI Programming Cookbook](https://www.packtpub.com/application-development/qt5-c-gui-programming-cookbook), by [Lee Zhi Eng](https://www.zhieng.com) [:octocat:](https://github.com/PacktPublishing/Qt5-C-GUI-Programming-Cookbook) - Overview of advanced GUI programming techniques for those familiar (but not satisfied) with the basics.  The source code used in the book is available for free.
- [Game Programming Using Qt: Beginner's Guide](https://www.packtpub.com/game-development/game-programming-using-qt) by Witold Wysota and Lorenz Haas - Good place to start learning how to program games with QML.
- [Application Development with Qt Creator - 2nd Edition](https://www.packtpub.com/application-development/application-development-qt-creator-second-edition), by [Ray Rischpater](http://www.lothlorien.com/kf6gpe) - Beginner's guide to Qt, with a lot of focus on Qt Creator and its associated tools.
- [Qt 5 Blueprints](https://www.packtpub.com/application-development/qt-5-blueprints), by [Symeon Huang](https://github.com/librehat) - Seems to be about the overall structure of a Qt project.
- [Mastering Qt 5](https://www.packtpub.com/application-development/mastering-qt-5), by [Guillaume Lazar](https://github.com/GuillaumeLazar) and [Robin Penea](https://github.com/synapticvoid) [:octocat:](https://github.com/PacktPublishing/Mastering-Qt-5) - Not your daddy's Qt.  Tips and tricks for the experienced.  The source code used in the book is available for free.
- [PySide GUI Application Development - 2nd Edition](https://www.packtpub.com/application-development/pyside-gui-application-development-second-edition), by Gopinath Jaganmohan and Venkateshwaran Loganathan - Imagine these other books, but in Python.
- [Qt5 Cadaques](https://qmlbook.github.io) [:octocat:](https://github.com/qmlbook/qmlbook) - Free book that focuses on QML, named for this town in northeastern Spain that the authors vacationed to once.

## Software that Uses Qt

A framework is only as great as the software that uses it.  Fortunately, much great software uses Qt.

- [Autodesk Maya](http://www.autodesk.com/maya) - 3D animation and design software that has been used to create visual effects for some of the most popular movies and TV shows of all time.
- [CMake](https://cmake.org) [:octocat:](https://github.com/Kitware/CMake) - The closest thing to a standard C++ build system out there. The bundled GUI uses Qt.
- [CRYENGINE](https://www.cryengine.com) [:octocat:](https://github.com/CRYTEK-CRYENGINE/CRYENGINE) - But can it run Crysis?  Some auxillary tools use Qt.
- [Doxygen](https://www.stack.nl/~dimitri/doxygen) [:octocat:](https://github.com/doxygen/doxygen) - The most popular documentation generator for C++, though it supports other languages as well.  The bundled GUI uses Qt.
- [Google Earth](https://www.google.com/earth) - *The* virtual globe.
- [KDE](https://www.kde.org) [:octocat:](https://github.com/KDE) - One of the most popular desktop environments for Linux.
- [Malwarebytes](https://www.malwarebytes.com) - Your Windows desktop's personal bodyguard.
- [Parallels Desktop](https://www.parallels.com/products/desktop) - Consumer-focused virtualization.
- [Qt Creator](https://www.qt.io/ide) [:octocat:](https://github.com/qtproject/qt-creator) - Something something eating your own dog food. Listed in the [official tools](#official-tools), but not listing it here doesn't feel right.
- [Rolisteam](http://www.rolisteam.org) [:octocat:](https://github.com/Rolisteam/rolisteam) - Virtual tabletop for remote Role Playing Games.
- [RUBE](https://www.iforce2d.net/rube) - Level design tool for any game that uses the Box2D physics engine.
- [TeamSpeak](https://www.teamspeak.com) - When gamers want to voice chat in a game that doesn't support it, they'll use this.
- [Telegram Desktop](https://desktop.telegram.org) [:octocat:](https://github.com/telegramdesktop/tdesktop) - Secure your conversations so well, you'll raise the blood pressure of potential eavesdroppers.  The desktop client uses Qt and is open source.
- [Tiled](http://www.mapeditor.org) [:octocat:](https://github.com/bjorn/tiled) - Perhaps the world's most popular tilemap editor.  Suitable for level design in games.
- [VirtualBox](https://www.virtualbox.org) [:package:](https://www.virtualbox.org/browser/vbox/trunk) - Virtualization software for x86/64 processors.  The bundled GUI uses Qt.
- [VLC](https://www.videolan.org/vlc) [:package:](https://code.videolan.org) - One of the most flexible open source video players in existence.
- [Vuo](https://vuo.org) [:octocat:](https://github.com/vuo/vuo) — Realtime visual programming language for interactive media.
- [Wireshark](https://www.wireshark.org) [:package:](https://code.wireshark.org/review/gitweb?p=wireshark.git;a=tree) - The most popular packet-sniffer out there.  You *are* going to use this for good and not evil, right?
- [Wolfram Mathematica](https://www.wolfram.com/mathematica) - Programming language, symbolic calculator, and an engineer's best friend.
- [Yabause](https://yabause.org) [:octocat:](https://github.com/Yabause/yabause) - Sega Saturn emulator.

There's also an official showroom [here](https://showroom.qt.io), which lets developers submit their own Qt-powered applications for display.

## Other Relevant Awesome Lists

If you're familiar with Awesome, you'll know that there's an *extremely* wide variety of resources, the usefulness of which will depend on your project.  However, if you're developing Qt applications, you'll almost certainly want to look at these as well.

- [Awesome C/C++](https://github.com/fffaraz/awesome-cpp) - There's no reason you can't use C++ libraries that weren't designed for Qt.  Sometimes they might even suit your needs better than what Qt offers.
- [Awesome C](https://github.com/aleksandar-todorovic/awesome-c) - Same goes for C libraries; might wanna brush up on those RAII techniques while you're at it.
- [Awesome CMake](https://github.com/onqtam/awesome-cmake) - If you're not using qmake for your project, you're likely using CMake instead.
- [Awesome OpenGL](https://github.com/eug/awesome-opengl) - Qt is commonly used for graphics applications, even providing its own wrappers around OpenGL.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, [Jesse Talavera-Greenberg](https://jessetg.github.io) has waived all copyright and related or neighboring rights to this work.  See the [LICENSE](LICENSE) file for details.
