# Android Google Play Services Ads version 15.0.0
Eclipse library projects based on the android google-play-services-ads 15.0.0 AAR release:
https://maven.google.com/com/google/android/gms/play-services-ads/15.0.0/play-services-ads-15.0.0.aar

It is old style eclipse library projects, which pack all the necessary libraries to run Google Mobile Ads, so there is no need to download and setup aditional dependencies. You don't need Gradle or Maven to build and use it.

The project is based on the work of https://github.com/dandar3/android-google-play-services-ads but the difference is that it packs all needed dependencies for working with Ads in one single git repository.
It supports banner and interstitial ads, represented by the following classes:

1. com.google.android.gms.ads.MobileAds
2. com.google.android.gms.ads.AdView
3. com.google.android.gms.ads.InterstitialAd
4. com.google.android.gms.ads.AdListener
5. com.google.android.gms.ads.AdRequest
6. com.google.android.gms.ads.AdSize

## How to use it

1. Download the distribution and extract the projects on the file system
2. Import the projects in Eclipse as existing library projects
3. Put a reference to the android-google-play-services-ads project from your Eclipse application project
4. Call MobileAds.initialize(this, "YOUR_ADMOB_APP_ID") in your Application onCreate method
5. Import interstitial activity in your AndroidManifest.xml: activity android:name="com.google.android.gms.ads.AdActivity"
     android:configChanges="keyboard|keyboardHidden|orientation|screenLayout|uiMode|screenSize|smallestScreenSize"
     android:exported="false"
     android:theme="@android:style/Theme.Translucent"
6. Implement your ads functionality using the com.google.android.gms.ads.AdView and com.google.android.gms.ads.InterstitialAd in your code
7. Run it

## References
https://firebase.google.com/docs/admob/android/quick-start

## About
I hope it will be helpful for somebody. If you like the project, please give it a star.
