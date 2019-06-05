# Android Google Play Services Ads version 17.2.1
Eclipse library projects based on the android google-play-services-ads 15.0.0 AAR release:
https://maven.google.com/com/google/android/gms/play-services-ads/15.0.0/play-services-ads-15.0.0.aar

It is old style eclipse library projects, which packs all the necessary projects to run Google Mobile Ads, so there is no need to download and setup aditional dependencies. You don't need Gradle or Maven to build and use it.

The project was created by merging different android archives, their classes and resources.
The R.class files are not presented for now so only limited functionality is available. It supports the old implementations of banner and interstitial ads, represented by the following classes:
1. com.google.android.gms.ads.AdListener
2. com.google.android.gms.ads.AdRequest
3. com.google.android.gms.ads.AdSize
4. com.google.android.gms.ads.AdView
5. com.google.android.gms.ads.InterstitialAd

## How to use it

1. Download the project
2. Rename the project folder to GPS_Ads_17.2.1 and import it to the Eclipse workspace
3. Put reference to the project from your Eclipse application project
4. Remove android-support-v4.jar (if exists) from the libs folder of your Eclipse application project in order to remove the duplicated classes
5. Import interstitial activity in your AndroidManifest.xml:
activity android:name="com.google.android.gms.ads.AdActivity"
     android:configChanges="keyboard|keyboardHidden|orientation|screenLayout|uiMode|screenSize|smallestScreenSize"
     android:exported="false"
     android:theme="@android:style/Theme.Translucent"
6. Implement your ads functionality using the com.google.android.gms.ads.AdView and com.google.android.gms.ads.InterstitialAd in your code
7. Run it

## About
I hope it will be helpful for somebody. If you like the project, please give it a star.
