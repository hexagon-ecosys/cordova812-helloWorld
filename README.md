This project helps reproduce an issue where cordova-plugin-device@2.1.0 breaks existing projects that (npm tilde) reference ~2.x.x and use Cordova versions < 9.

To reproduce -

1. npm install cordova@8.1.2 (-g)
2. cd <this project>
3. npm install
4. cordova prepare

The error is as follows -
  
Failed to restore plugin "cordova-plugin-device" from config.xml. You might need to try adding it again. Error: code: engine.platform or engine.scriptSrc is not defined in custom engine "cordova-electron" from plugin "cordova-plugin-device" for android warn
