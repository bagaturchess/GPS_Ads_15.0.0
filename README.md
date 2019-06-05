# Android Google Play Services Ads version 17.2.1
Eclipse library project based on the android google-play-services-ads 17.2.1 AAR release:
https://maven.google.com/com/google/android/gms/play-services-ads/17.2.1/play-services-ads-17.2.1.aar

It is old style eclipse library project which packs all the necessary libraries into the libs folder, so there is no need to download and setup aditional dependencies. You don't need Gradle or Maven to build and use it.

The project was created by a lot of manual work - merging of different android archives, their classes and resources.
I hope it will be helpful for somebody. If you like the project, please give it a star.

## How to use it

1. Download the project
2. Rename the project folder to GPS_Ads_17.2.1 and import it to the Eclipse
3. Put reference to the project from your Eclipse application project
4. Remove android-support-v4.jar (if exists) from the libs folder of your Eclipse application project
5. Run it
