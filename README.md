# Official Release 1.0.0 - 6/Nov/17
[Android Developers Blog](https://android-developers.googleblog.com/2017/11/announcing-architecture-components-10.html)

> Prior to the release of Android Architecture Components we had our own ViewModel implementation. We used Loaders and Dependency Injection to persist our ViewModel through config changes.

> We've also started to use LiveData which hooks directly into the Activity lifecycle. We use it to retrieve and display network data and no longer have to concern ourselves with ​network call subscription management.

# [Why MVVM over MVP?](https://www.reddit.com/r/androiddev/comments/7cp0xn/mvc_vs_mvp_vs_mvvm_vs_mvi/dpssidd/)

> What about config changes, like screen orientation change while http requests are running? How do you restore that "state" (showing progress bar because http request is still running after screen orientation change) in MVP ?

> What about back stack navigation like starting http request in Fragment A, but then navigate to Fragment B (Fragment A is not visible anymore, it's on the back stack, hence Presenter of Fragment A has no view attached).

> What about more complex screens like a list of items displayed in a recyclerview but your user can do a pull to refresh and pagination (load more items when the user has scrolled to the end of the recyclerview) at the same time. How do you do that in MVP? Now add screen orientation changes and backstack navigation to that equation. Easy, right?

> Sure somehow you can implement it in MVP but how maintainable is that code? That kind of problems can be solved with "state management"

# Components

1) Lifecycles
2) LiveData
3) ViewModel
4) Room
5) _Paging Library (still in alpha)_

# Videos

01) [_17/May/17_] | [**05:41**] | [Architecture Components: Improve Your App's Design - Lyla](https://www.youtube.com/watch?v=vOJCrbr144o) Google I/O 17
02) [_17/May/17_] | [**38:26**] | [Architecture Components - Introduction - Mike, Yigit, Lukas](https://www.youtube.com/watch?v=FrteWKKVyzI) Google I/O 17
03) [_18/May/17_] | [**39:30**] | [Architecture Components - Persistence and Offline - Yigit, Kirill](https://www.youtube.com/watch?v=MfHsPGQ6bgE) Google I/O 17
04) [_18/May/17_] | [**35:42**] | [Architecture Components - Solving the Lifecycle Problem - Sergey, Adam, Yigit](https://www.youtube.com/watch?v=bEKNi1JOrNs) Google I/O 17
05) [_02/Aug/17_] | [**19:30**] | [Data Persistence In Android: Room For Improvement - Florina](https://academy.realm.io/posts/360-andev-2017-florina-muntenescu-data-persistence-android-room/) Conference: 360|AnDev
06) [_30/Aug/17_] | [**47:55**] | [Architecture Components – Behind the Scenes - Yigit](https://www.youtube.com/watch?v=2QDAbH2tdoE) Conference: 360|AnDev
07) [_06/Sep/17_] | [**05:16**] | [MVVM + RxJava - Florina](https://www.youtube.com/watch?v=h25FDyGTLso) Android Dialogs
08) [_06/Sep/17_] | [**20:21**] | [Architecture Components - Florina](https://www.youtube.com/watch?v=Ts-uxYiBEQ8) GDD Europe '17
09) [_18/Oct/17_] | [**19:30**] | [Data Persistence In Android - Florina](https://www.youtube.com/watch?v=DeIKyVfCvC0) Conference: DroidcOn Berlin
10) [_31/Oct/17_] | [**40:47**] | [ViewModels, LiveData and Lifecycles, oh my! - Lyla](https://www.youtube.com/watch?v=SlZVYkhoSq8) Conference : Droidcon NYC 17
11) [_31/Oct/17_] | [**38:32**] | [Clean app design with Architecture Components - Chuck](https://www.youtube.com/watch?v=i1-7S-RxfvQ) Conference : Droidcon NYC 17
12) [_31/Oct/17_] | [**42:03**] | [Android Architecture Round Table - Yigit, Mike, Lucia, Israel, Mike, Micheal, Annyce, Jake, Jose](https://www.youtube.com/watch?v=nP_B5-jrbsY) Conference : Droidcon NYC 17
13) [_06/Nov/17_] | [**03:59**] | [Architecture Components: Room - Florina](https://www.youtube.com/watch?v=H7I3zs-L-1w) Official stable 1.0.0 release video
14) [_08/Nov/17_] | [**04:51**] | [Architecture Components: ViewModel - Lyla](https://www.youtube.com/watch?v=c9-057jC1ZA) Official Android Developer
15) [_10/Nov/17_] | [**05:15**] | [Architecture Components: LiveData and Lifecycle - Lyla](https://www.youtube.com/watch?v=jCw5ib0r9wg) Official Android Developer

# Podcasts

01) [_18/Sep/17_] | [**35:36**] | [Android Architecture Paging Library - Florina](http://fragmentedpodcast.com/episodes/97/) Fragmented Podcast E97
02) [_18/Jul/17_] | [**51:53**] | [Architecture Components 2 - Persistence - Yigit, Sergei](http://androidbackstage.blogspot.com/2017/07/episode-73-architecture-components-2.html) Android Developer Backstage E73
03) [_30/Jun/17_] | [**43:52**] | [Architecture Components 1 - Lifecycle - Yigit, Sergei](http://androidbackstage.blogspot.com/2017/06/episode-72-architecture-components-1.html) Android Developer Backstage E72


# Samples

1) [_09/May/17_] | [:star2: 4729] | **Official** - Android Architecture Components : https://github.com/googlesamples/android-architecture-components
2) [_16/Aug/17_] | [:star2: 20] | **Official** - Google Code Labs : https://codelabs.developers.google.com/codelabs/build-app-with-arch-components/index.html
3) [_11/Apr/16_] | [:star2: 146] | Florina - Hello World : https://github.com/florina-muntenescu/MVPvsMVVM
4) [_08/Nov/17_] | [:star2: 6] | 3rd Party - MovieNight : https://github.com/TwistedMetalGear/MovieNight
5) [_19/May/17_] | [:star2: 166] | 3rd Party - Kucherenkolhar : https://github.com/KucherenkoIhor/Android-Architecture-Components
6) [_21/May/17_] | [:star2: 474] | 3rd Party - ArchMovie : https://github.com/iammert/AndroidArchitecture



### 1- Official Google -> [android-architecture](https://github.com/googlesamples/android-architecture)

#### 1a [Github Browser Sample](https://github.com/googlesamples/android-architecture-components/tree/master/GithubBrowserSample/app/src/main/java/com/android/example/github) **9-May-17 | :star2: 4729**

1) P+L(Config-chages-sup)
----
### 2- Official Google -> [Code Labs](https://codelabs.developers.google.com/?cat=Android)

#### 2a [Android lifecycle-aware components codelab](https://github.com/googlecodelabs/android-lifecycles/tree/master/app/src/main/java/com/example/android/lifecycles) **5-Sep-17**

1) P+L(Config-chages-sup)

#### 2b [Build an app with Architecture Component](https://github.com/googlecodelabs/android-build-an-app-architecture-components/tree/arch-training-steps/app/src/main/java/com/example/android/sunshine) **4-Sep-17**

1) P+L(Config-chages-sup)

#### 2c [Android Persistence codelab](https://github.com/googlecodelabs/android-persistence) **3-Sep-17**

1) P+L(Config-chages-sup)

----

### 3- 3rd Party -> [Florina - Hello World](https://github.com/florina-muntenescu/MVPvsMVVM/tree/master/app/src/main/java/upday/mvpvsmvvm) **11-Apr-16 | :star2: 146**

1) P+L(Config-chages-sup)
----

### 4- 3rd Party -> [MovieNight](https://github.com/TwistedMetalGear/MovieNight/tree/master/app/src/main/java/net/silentbyte/movienight) **8-Nov-17 | :star2: 16**

[Reddit](https://www.reddit.com/r/androiddev/comments/7bh4vd/movie_night_a_simple_movie_app_showcasing_android/)

1) P+L(Config-chages-sup)
----

### 5- 3rd Party -> [Kucherenkolhar](https://github.com/KucherenkoIhor/Android-Architecture-Components/tree/master/app/src/main/java/com/ik/exploringviewmodel) **19-May-17 | :star2: 176**

1) P+L(Config-chages-sup)
2) Kotlin
----

### 6- 3rd Party -> [ArchMovie](https://github.com/iammert/AndroidArchitecture/tree/master/app/src/main/java/iammert/com/androidarchitecture) **21-May-17 | :star2: 476**

1) P+L(Config-chages-sup)
2) LiveData, Room Persistence, Dagger 2, Retrofit, MVVM, DataBinding
3) View Pager
----

# Links

**Forum**
1) Android Developers Blog - [Announcing Architecture Components 1.0 Stable](https://android-developers.googleblog.com/2017/11/announcing-architecture-components-10.html)
2) Reddit MY - [Android Architecture Component - TODO GUIDE](https://www.reddit.com/r/androiddev/comments/7bbs5s/shanraisshanandroidarchitecturecomponentstodoguide/)
3) Reddit MY - [Android Architecture Component with View Pager](https://www.reddit.com/r/androiddev/comments/7bl1t8/android_architecture_components_example_using/)

**Tutorials**
1) [ViewModels : A Simple Example](https://medium.com/google-developers/viewmodels-a-simple-example-ed5ac416317e) | [Github](https://github.com/udacity/Court-Counter)
2) [ViewModels: Persistence, onSaveInstanceState(), Restoring UI State and Loaders](https://medium.com/google-developers/viewmodels-persistence-onsaveinstancestate-restoring-ui-state-and-loaders-fc7cc4a6c090)
