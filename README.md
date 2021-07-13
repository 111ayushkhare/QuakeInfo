# QuakeInfo

## App description
* An android app **(Kotlin)** fetches earthquake data from a network call to an API. 
* This app follows the **Android's Model-View-ViewModel, i.e., MVVM architecture** with the implementation of **data-binding**. 
* It has a **Range-Slider** depicting earthquake magnitude range (eathquakes with magnitudes in this selected range only will be fetched and displayed).
* Fetching the earthquake data is done in a background thread without blocking the UI thread with help of **Kotlin-Coroutines**. 
* The app uses **Retrofit-library** for calling and setting up the API service and **Moshi-converter** for decoding the fetched the **JSON data**. 
* The fetched data is displayed in a **Recycler view** where each item is **card view** conatining Magnitude, Location, Date and Time of the earthquake.
* The app has two fragments - Earthquake Overview Fragment & Earthquake Detail Fragment (left). Navigation between these two fragmets is done by implementing **Android's Jetpack Navigation**.
* Different color schemes for light and dark themes.

## Demo of app working

### Overview Screen
<br />

<p>
  <img src="https://user-images.githubusercontent.com/46900324/125501799-f51ff574-6363-4045-afe8-ee7e401160fe.gif" width="300" height="600" />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://user-images.githubusercontent.com/46900324/125501909-ff89c339-c868-4501-ad60-18e8964f64ef.gif" width="300" height="600" /> 
</p>

## Data Source
* USGS website - [https://earthquake.usgs.gov/](https://earthquake.usgs.gov/)
* USGS API used - [https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minmagnitude=1.0&maxmagnitude=10.0](https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minmagnitude=6&maxmagnitude=10.0)<br />
