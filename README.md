# RandomMovie
 "RandomMovie" is an Android application that draws random movies and gives users the ability to mark favorites as favorites. The app allows users to discover randomly selected movies, find ones that interest them, and add them to their favorites list. This can be used as a handy tool to help you discover and get recommended movies more easily.



# API calls and responses

The process of calling the API and processing the response is as follows:

Issue an API key:
Register as a developer at TMDb and receive an API key. This key is required when calling the API.
This allows the Random Movie project to dynamically retrieve movie data and display it on the screen.
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


## Movie API

This Kotlin code defines data classes for representing movie information through an API.

```kotlin
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
```


This is a data class written using the Kotlin programming language. These classes define data that can be used to represent movie information. The classes used here are:

1. **MovieApi**: This class represents key information in the movie. It has the following properties:
   - `titleText`: An object of type `TitleTextApi` representing the movie title..
   - `releaseYear`: An object of type `ReleaseYearApi` representing the release year of the movie..
   - `primaryImage`: It is an object of type `PrimaryImageApi` representing the main image information of the movie..

2. **PrimaryImageApi**: This class represents information about the featured image. There is one attribute, `url`, which represents the URL of the image.

3. **TitleTextApi**: This class represents information about the movie title. There is one property, `text`, which is a string representing the title of the movie.

4. **ReleaseYearApi**: This class represents information about the release year of a movie. There is one property, `year`, which is an integer value representing the year of release.

## Movie Service

This Kotlin code defines a Retrofit service interface for interacting with a movie API.

```kotlin
package com.example.randommovie.api.service

import com.example.randommovie.api.model.MovieListApi
import io.reactivex.rxjava3.core.Single
import retrofit2.http.GET
import retrofit2.http.Query

interface MovieService {

    @GET("titles/random")
    fun getRandomMovies(
        @Query("list") list: String,
        @Query("limit") limit: Int
    ): Single<MovieListApi>
}

```
``` kotlin
MovieService The interface is used to interact with the Movie API using Retrofit.
The @GET("titles/random") annotation performs an HTTP GET request, with an endpoint of "titles/random".
The getRandomMovies function takes two query parameters, sends a request to the API, and uses Single<MovieListApi> as the return value. It represents the result of an asynchronous operation using the Single class provided by RxJava.
@Query("list") list: String and @Query("limit") limit: Int represent query parameters to be included in the GET request.
```
# Results
`

<img width="310" alt="Screenshot 2023-12-06 at 9 51 10 PM-2" src="https://github.com/YokubovMukhammadali/randommovie-android/assets/119654152/78bb6af5-adfa-4a59-b034-1252e94c4c38">

<img width="290" alt="Screenshot 2023-12-06 at 9 51 10 PM-2" src="https://github.com/YokubovMukhammadali/randommovie-android/assets/119654152/d574f01e-9eb7-45d1-8ecd-379c7a044cdd">

<img width="290" alt="Screenshot 2023-12-06 at 9 51 10 PM-2" src="https://github.com/YokubovMukhammadali/randommovie-android/assets/119654152/f0f56a8b-451f-48d9-b2ec-0d201256a58f">

## Video


<video width="290" alt="Screenshot 2023-12-06 at 9 51 10 PM-2" src="https://github.com/YokubovMukhammadali/randommovie-android/assets/119654152/1a8a3907-020e-4b17-9d96-abd54ae68700">
```

## Author

Student number: 21102454 Name: Mukhammadali





