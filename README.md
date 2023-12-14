# RandomMovie
 "RandomMovie" is an Android application that draws random movies and gives users the ability to mark favorites as favorites. The app allows users to discover randomly selected movies, find ones that interest them, and add them to their favorites list. This can be used as a handy tool to help you discover and get recommended movies more easily.

# Movie Data API   

Introduction to the APIs used

The Random Movie project uses The Movie Database (TMDb) API to dynamically retrieve various movie information and display it on the screen. The TMDb API provides a variety of data, including information about movies, posters, and reviews.

# API calls and responses

The process of calling the API and processing the response is as follows:

Issue an API key:
Register as a developer at TMDb and receive an API key. This key is required when calling the API.
This allows the Random Movie project to dynamically retrieve movie data and display it on the screen.

# Results
## Find your favorite movies: Find your favorite movies.
### About the app:

"RandomMovie is a movie recommendation app that runs on the Android platform."
“You can manage your movies by receiving random movie recommendations.”
By rating your favorite movies, you can use them as a reference when choosing movies in the future. Random movies always offer unexpected aspects and unique insights. Diverse themes and diverse characters allow you to observe the world from new angles, which leads to the opportunity to gain deeper understanding and awareness. Random movies provide a rich visual experience that takes you out of your daily routine and inspires you.

# Conclusion and Acknowledgments
## Project Importance

The Random Movie project gave me valuable experience learning and applying new techniques.
By integrating the movie data API, we experienced interacting with real data and were able to build on our knowledge in various aspects of Android app development.
future prospects

The project is continuously evolving, and additional features and improvements are being considered.
Through user feedback, we are planning upgrades to improve the app's user experience, include more movie data, and more.

mmmmmmm

''' kotlin
package com.example.randommovie.api.model

data class MovieApi(
    val titleText: TitleTextApi?,
    val releaseYear: ReleaseYearApi?,
    val primaryImage: PrimaryImageApi?
)

data class PrimaryImageApi(
    val url: String?
)

data class TitleTextApi(
    val text: String?
)

data class ReleaseYearApi(
    val year: Int?
)
이것은 Kotlin 프로그래밍 언어를 사용하여 작성된 데이터 클래스입니다. 이 클래스들은 영화 정보를 표현하는 데 사용될 수 있는 데이터를 정의합니다. 여기에 사용된 클래스들은 다음과 같습니다:

1. **MovieApi**: 이 클래스는 영화의 주요 정보를 나타냅니다. 다음과 같은 속성들을 가지고 있습니다:
   - `titleText`: 영화 제목을 나타내는 `TitleTextApi` 형식의 객체입니다.
   - `releaseYear`: 영화의 출시 연도를 나타내는 `ReleaseYearApi` 형식의 객체입니다.
   - `primaryImage`: 영화의 주요 이미지 정보를 나타내는 `PrimaryImageApi` 형식의 객체입니다.

2. **PrimaryImageApi**: 이 클래스는 주요 이미지에 대한 정보를 나타냅니다. 하나의 속성인 `url`이 있으며, 이는 이미지의 URL을 나타냅니다.

3. **TitleTextApi**: 이 클래스는 영화 제목에 대한 정보를 나타냅니다. 하나의 속성인 `text`가 있으며, 이는 영화 제목을 나타내는 문자열입니다.

4. **ReleaseYearApi**: 이 클래스는 영화의 출시 연도에 대한 정보를 나타냅니다. 하나의 속성인 `year`가 있으며, 이는 출시 연도를 나타내는 정수값입니다.

이 코드는 주로 Kotlin에서 JSON 또는 다른 형식의 데이터를 쉽게 파싱하거나 표현하기 위해 사용될 수 있습니다. 예를 들어, 이 데이터 클래스들은 Retrofit이나 Gson 같은 라이브러리를 사용하여 서버에서 받아온 JSON 데이터를 객체로 변환할 때 편리하게 사용될 수 있습니다.
'''






<img width="310" alt="Screenshot 2023-12-06 at 9 51 10 PM-2" src="https://github.com/YokubovMukhammadali/randommovie-android/assets/119654152/78bb6af5-adfa-4a59-b034-1252e94c4c38">

<img width="290" alt="Screenshot 2023-12-06 at 9 51 10 PM-2" src="https://github.com/YokubovMukhammadali/randommovie-android/assets/119654152/d574f01e-9eb7-45d1-8ecd-379c7a044cdd">

<img width="290" alt="Screenshot 2023-12-06 at 9 51 10 PM-2" src="https://github.com/YokubovMukhammadali/randommovie-android/assets/119654152/f0f56a8b-451f-48d9-b2ec-0d201256a58f">

## Video


<video width="290" alt="Screenshot 2023-12-06 at 9 51 10 PM-2" src="https://github.com/YokubovMukhammadali/randommovie-android/assets/119654152/1a8a3907-020e-4b17-9d96-abd54ae68700">





