# Adcash MoPub Adapter iOS

This SDK is designed for integrating Adcash with MoPub Mediation on iOS to maximize fill rate and revenue.

It's a simple 2-step process.

# Integration Guide

**Note :** Assuming integration is already done with MoPub SDK, if not please follow [MoPub Integration guideline](https://dev.twitter.com/mopub/ios/getting-started).

## 1. Download SDK

+ Download the Adcash SDK [here](https://github.com/adcash/Adcash-MoPub-Adapter-iOS).
+ Drag and drop the file into your Xcode project.
+ Don't forget to check "Copy items if needed"

![](http://developer.adca.sh/wp-content/uploads/2016/08/ScreenShot1.png)

## 2. Configure Adcash Custom Event on MoPub Mediation Portal

### 2.1. Add a Network

On MoPub Dashboard, click on **Networks** tab, then click on **Add a Network** button.

![](http://i0.wp.com/developer.adca.sh/wp-content/uploads/2016/09/ScreenShot2.png)

On the **Add a Network** page, select **Custom Native Network** under **Additional Networks** section.

![](http://i1.wp.com/developer.adca.sh/wp-content/uploads/2016/09/ScreenShot3.png)

### 2.2 Configure Custom Native Ad Network

Give it a title **Adcash**, then scroll down for ad units (Adcash MoPub iOS Adapter currently supports Banner and Interstitial ad formats)

Custom Event Information from:
* **Custom Event Class**
- For Banner: "AdcashMopubBanner"
- For Interstitial: "AdcashMopubInterstitial"
* **Custom Event Class Data:**
- Enter your Zone ID from Adcash Publisher Panel. It has to be in JSON format

> example : {"id":"your_zone_id"}


![](http://developer.adca.sh/wp-content/uploads/2016/09/ScreenShot41.png)

## 3. Release App

Now Adcash is successfully has integrated with MoPub Mediation platform and you can release out the app in iTunes. Please note that changes made in MoPub Portal might take couple hours to reflect.
