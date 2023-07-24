# Firetv development documentation

A. How to test the in-app purchase in Amazon FireTV?
   1. Download the Amazon app tester from the Amazon store in FireTV
   2. Then use below JSON file path for running the cmd command > adb push D:\RS\amazon.sdktester.json /mnt/sdcard/amazon.sdktester.json
   3. Export sdktester.json from 'developer.amazon.com, under In-App Items >  'Export Multiple IAPs'
   4. Once the above steps over then use cmd command > adb shell setprop debug.amazon.sandboxmode debug
   5. Then run the app for subscription flow
   6.  Once, the testing over, then run > adb shell setprop debug.amazon.sandboxmode none
