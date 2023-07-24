# Firetv development documentation

A. How to test the in-app purchase in Amazon FireTV?
   1. Download the Amazon app tester from the Amazon store in FireTV
   2. Then use below JSON file path for running the cmd command > adb push D:\RS\amazon.sdktester.json /mnt/sdcard/amazon.sdktester.json
   3. Export sdktester.json from 'developer.amazon.com, under In-App Items >  'Export Multiple IAPs'
   4. Just for reverifying sdktester.json, open ' Amazon app tester' in firetv and go to 'IAP Items in JSON File'. It should show the purchase-related info.
   5. Once the above steps over then use cmd command > adb shell setprop debug.amazon.sandboxmode debug
   6. Then run the app for subscription flow
   7.  Once, the testing over, then run > adb shell setprop debug.amazon.sandboxmode none
