# Firetv_doc

1. How to test the in-app purchase in Amazon FireTV?
   > Download the Amazon app tester from the Amazon store in FireTV
   > Then use below JSON file path for running the cmd command > adb push D:\RS\amazon.sdktester.json /mnt/sdcard/amazon.sdktester.json
   > Export sdktester.json from 'developer.amazon.com, under In-App Items >  'Export Multiple IAPs'
   > Once the above steps over then use cmd command > adb shell setprop debug.amazon.sandboxmode debug
   > Then run the app for subscription flow
   > Once, the testing over, then run > adb shell setprop debug.amazon.sandboxmode none
