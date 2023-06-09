# GitHub Pull Requests App :octocat:

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&amp;logo=flutter&amp;logoColor=white)
![Last Commit](https://img.shields.io/github/last-commit/kingavatar/github-pr-dashboard)
![Code Size](https://img.shields.io/github/languages/code-size/kingavatar/github-pr-dashboard)
![Top Language](https://img.shields.io/github/languages/top/kingavatar/github-pr-dashboard)
<!--- ![License](https://img.shields.io/github/license/kingavatar/github-pr-dashboard) --->


This Flutter app displays a list of pull requests from a GitHub repository, which can be sorted and filtered based on various parameters. The app features animated Lottie asset icons that provide visual feedback to the user, as well as handling edge cases such as 404 errors and loading states with attractive Lottie animations. The app includes settings to handle confirm-on-exit for both Android and iOS, as well as theme modes and dynamic colors using Material You. The latest Material 3 components are used throughout the app.

## Features :sparkles:

- Display a list of pull requests from a GitHub repository
- Sort and filter pull requests based on various parameters
- View detailed information about a pull request in a separate page
- Animated Lottie asset icons for visual feedback and loading states
- Handle 404 errors and other edge cases with attractive Lottie animations
- Confirm-on-exit settings for Android and iOS
- Theme modes and dynamic colors using Material You
- Latest Material 3 components used throughout the app
- Infinite scrolling to handle pagination

## Dependencies :package:

This app utilizes the following dependencies:

- [Dio](https://pub.dev/packages/dio) ![Dio](https://img.shields.io/badge/Dio-^5.1.1-009688?style=for-the-badge&amp;logo=dio&amp;logoColor=white) for handling network API calls
- [Flutter Riverpod](https://pub.dev/packages/flutter_riverpod) ![Riverpod](https://img.shields.io/badge/Riverpod-^2.3.5-0D47A1?style=for-the-badge&amp;logo=riverpod&amp;logoColor=white) for state management
- [cached_network_image](https://pub.dev/packages/cached_network_image) ![Cached Network Image](https://img.shields.io/badge/cached_network_image-^3.2.3-00BFFF?style=for-the-badge&amp;logo=cached_network_image&amp;logoColor=white) to cache avatar images from the GitHub API
- [lottie](https://pub.dev/packages/lottie) ![Lottie](https://img.shields.io/badge/Lottie-^2.3.2-FF4081?style=for-the-badge&amp;logo=lottiefiles&amp;logoColor=white) for animated icons
- [package_info_plus](https://pub.dev/packages/package_info_plus) ![Package Info Plus](https://img.shields.io/badge/package_info_plus-^3.1.0-FFC107?style=for-the-badge&amp;logo=package_info_plus&amp;logoColor=white) for getting information about the app package
- [cupertino_icons](https://pub.dev/packages/cupertino_icons) ![](https://img.shields.io/badge/cupertino_icons-^1.0.2-000000?style=for-the-badge&amp;logo=cupertino_icons&amp;logoColor=white) for using iOS-style icons
- [beamer](https://pub.dev/packages/beamer) ![Beamer](https://img.shields.io/badge/Beamer-^1.5.3-FF9800?style=for-the-badge&amp;logo=beamer&amp;logoColor=white) for implementing navigation and routing
- [flutter_svg](https://pub.dev/packages/flutter_svg) ![](https://img.shields.io/badge/flutter_svg-^2.0.5-E91E63?style=for-the-badge&amp;logo=flutter_svg&amp;logoColor=white) for rendering SVG images
- [timeago](https://pub.dev/packages/timeago) ![](https://img.shields.io/badge/timeago-^3.4.0-4CAF50?style=for-the-badge&amp;logo=timeago&amp;logoColor=white) for displaying human-readable timestamps
- [auto_size_text](https://pub.dev/packages/auto_size_text) ![](https://img.shields.io/badge/auto_size_text-^3.0.0-F44336?style=for-the-badge&amp;logo=auto_size_text&amp;logoColor=white) for dynamically sizing text
- [infinite_scroll_pagination](https://pub.dev/packages/infinite_scroll_pagination) ![](https://img.shields.io/badge/infinite_scroll_pagination-^3.2.0-9C27B0?style=for-the-badge&amp;logo=infinite_scroll_pagination&amp;logoColor=white) for implementing infinite scrolling with pagination
- [dynamic_color](https://pub.dev/packages/dynamic_color) ![](https://img.shields.io/badge/dynamic_color-^1.6.3-F9A825?style=for-the-badge&amp;logo=dynamic_color&amp;logoColor=white) for implementing dynamic colors based on user's wallpaper
- [flutter_exit_app](https://pub.dev/packages/flutter_exit_app) ![](https://img.shields.io/badge/flutter_exit_app-^1.1.2-CDDC39?style=for-the-badge&amp;logo=flutter_exit_app&amp;logoColor=white) for handling confirm-on-exit on Android and iOS


## Getting Started :rocket:

To set up the app, follow these steps:

1. Clone the repository:

```
git clone https://github.com/kingavatar/github-pr-dashboard.git
```

2. Install dependencies:

```
flutter pub get
```

<!--
 3. Create a `.env` file in the root directory of the project and add your GitHub personal access token:

```
GITHUB_API_TOKEN=<your token here>
```
-->

3. Run the app:

```
flutter run
```

## Architecture :building_construction:

The project follows a simple folder structure, with most of the code residing in the lib directory. The lib directory contains the main app code, with the following subdirectories:

screens: This directory contains all the screen widgets of the app. Each screen widget is self-contained and handles its own state and UI. Screens can be navigated using the navigation widgets in the widgets directory.
widgets: This directory contains common widgets used throughout the app, such as the navigation bar and navigation rail. The widgets in this directory are reusable and can be customized to fit the specific needs of each screen.
transitions: This directory contains the animation transitions used by the navigation widgets in the widgets directory. These transitions provide smooth and attractive animations when switching between screens.
In addition to the main app code, the project also utilizes several third-party libraries to handle network requests, state management, and image caching:

Dio is used to handle network API calls to the GitHub REST API. Dio is a powerful HTTP client for Dart that supports interceptors, global configuration, FormData, and more.
Riverpod is used for state management throughout the app. Riverpod is a simple yet powerful state management library for Flutter that provides a way to manage app state in a scalable and testable way.
cached_network_image is used to cache avatar images from the GitHub API. cached_network_image is a Flutter library that provides a way to cache images from the network using a simple API.
The app also features infinite scrolling to handle pagination, which is implemented using the Flutter built-in ListView.builder widget.

Finally, the app includes settings to handle confirm-on-exit for both Android and iOS, as well as theme modes and dynamic colors using Material You. The latest Material 3 components are used throughout the app to provide a modern and consistent UI.

Overall, the project follows a clean and organized architecture that separates concerns and promotes code reusability and maintainability.

## Design :art:

The app features a modern Material 3 design, utilizing the latest components and features. The app is designed to be both visually appealing and easy to use, with a focus on user experience.

One notable design feature of the app is the use of Material You dynamic colors. This feature enables the app to dynamically adjust its color scheme based on the user's device settings. On Android S+, the app will use the color from the user's wallpaper, while on Linux, the app will use the GTK+ theme's @theme_selected_bg_color. On macOS, the app will use the system accent color, and on Windows, the app will use the accent color or window/glass color.

The app also utilizes custom Lottie animations for visual feedback, including loading animations and error animations. The animations provide an attractive and engaging user interface, while also conveying important information to the user.

The app includes support for both light and dark modes, with appropriate color schemes for each mode. The theme can be easily changed from the app settings, allowing users to customize their experience.

Overall, the app is designed to be both aesthetically pleasing and easy to use, while also being maintainable and scalable for future development.

## Challenges :muscle:

One of the challenges in developing the app was handling pagination for the list of pull requests. This was addressed using infinite scrolling, which allowed the app to fetch new data as the user scrolled through the list.

Riverpod handled majority of cases for providing data from repository API calls to UI.

When enabling dark mode I had to transition all the lottie assets manually from black color to white color.

Search Page with errors with custom 404 page dealing while handling pagination made me rewrite most of the code.

BottomSheet still has some constraints needed to be handled. They are pending issues of max-width in flutter API. For now I handled using sizedBox and constrainedBox where needed.

Exiting the app was weirdly not handled using native methods which used native channels to handle the case. I has to use the flutter_exit_app to deal with that case.

Beamer, which was used for navigation and routing, also presented some challenges and took some time to get used to.

## Screenshots :camera_flash:

<table align="center">
<tr align="center">
    <td>Pull to Refresh</td>
     <td>Searching</td>
     <td>Filtering/Sorting</td>
</tr>
<tr>
<td><img src="https://raw.githubusercontent.com/kingavatar/github-pr-dashboard/assets/pulltorefresh.gif" width="200" /></td>
<td><img src="https://raw.githubusercontent.com/kingavatar/github-pr-dashboard/assets/wezterm.gif" width="200" /></td>
<td><img src="https://raw.githubusercontent.com/kingavatar/github-pr-dashboard/assets/filter.gif" width="200" /></td>
</tr>
</table>


<table align="center">
<tr align="center">
    <td>Details</td>
     <td>Animated Icons</td>
     <td>404</td>
</tr>
<tr>
<td><img src="https://raw.githubusercontent.com/kingavatar/github-pr-dashboard/assets/details.gif" width="200" /></td>
<td><img src="https://raw.githubusercontent.com/kingavatar/github-pr-dashboard/assets/animatedIcons.gif" width="200" /></td>
<td><img src="https://raw.githubusercontent.com/kingavatar/github-pr-dashboard/assets/404.gif" width="200" /></td>
</tr>
</table>


<table align="center">
<tr align="center">
    <td>DarkMode</td>
     <td>Dynamic</td>
     <td>Confirm To Exit</td>
</tr>
<tr>
<td><img src="https://raw.githubusercontent.com/kingavatar/github-pr-dashboard/assets/darkmode.gif" width="200" />  </td>
<td><img src="https://raw.githubusercontent.com/kingavatar/github-pr-dashboard/assets/dynamic.gif" width="200" />  </td>
<td><img src="https://raw.githubusercontent.com/kingavatar/github-pr-dashboard/assets/confirmToExit.gif" width="200" /> </td>
</tr>
</table>

<table align="center">
<tr align="center">
<td>Change Layout on Resize</td>
</tr>
<tr>
<td><img src="https://raw.githubusercontent.com/kingavatar/github-pr-dashboard/assets/resize.gif"/></td> 
</tr>
</table>

## Contributing :handshake:

If you are interested in contributing to the project, please follow these steps:

1. Fork the repository
2. Create a new branch for your feature or bug fix
3. Make your changes and commit them
4. Push your changes to your forked repository
5. Submit a pull request to the original repository

## Issues :bug:

If you encounter any issues with the app, please submit an issue on the GitHub repository page.
