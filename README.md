PaymentKit-Droid
================



To build the project:

./gradlew assembleDebug
./gradlew assembleRelease

- If you wanna publish to your own repo, lets say if you made some custom changes, set up the following Gradle properties in gradle.properties.
It can be found in one of two places:
1) vi ~/.gradle/gradle.properties, or
2) <project root>/gradle.properties

- sonatypeRepo (pointing to your Maven repo).
- sonatypeUsername (username to that repo)
- sonatypePassword (password to your repo)
- scmUrl (URL pointing to your Maven server. Example: 'scm:git@github.com:coomar2841/image-chooser-library.git')

chooserReleaseKeyAlias (the absolute path to the key store you wanna sign with). Example: /Users/donald/keystores/mykeystore.keystore.jks
chooserReleaseKeyPassword=<password>
chooserReleaseStoreFile=<store file>
chooserReleaseStorePassword=<store password>

To build and upload to your repo:
./gradlew uploadArchives



PaymentKit-Droid is an Open Source Android library that allows developers to create sleek payment forms like those made
popular by StubHub, Stripe, Uber, and Postmates. The library provides support for as far back as 2.1.

The PKExample provides an example implementation pattern you may follow.

Right now you'll need to add this project as a submodule project to Android Studio. 
For more information see http://www.ipreferjim.com/2013/06/android-studio-and-library-projects/

A sample app will soon be available on the google play store.

Feel free to leave requests and feedback through github (brendanw) or twitter (elbrendan).

You can also find my contact information at http://www.brendanweinstein.me

Things to be added in the future:

- Documentation
- AAR getting added to maven central
- Better handling of spacing for landscape mode
- Support for more cards
- More error messaging ability options 
# PaymentKit-Droid
