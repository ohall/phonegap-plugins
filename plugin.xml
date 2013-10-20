   1 <?xml version="1.0" encoding="UTF-8"?>
   2 
   3 <plugin xmlns="http://apache.org/cordova/ns/plugins/1.0"
   4     xmlns:rim="http://www.blackberry.com/ns/widgets"
   5     xmlns:android="http://schemas.android.com/apk/res/android"
   6     id="org.apache.cordova.device"
   7     version="0.2.3">
   8     <name>Device</name>
   9     <description>Cordova Device Plugin</description>
  10     <license>Apache 2.0</license>
  11     <keywords>cordova,device</keywords>
  12 
  13     <js-module src="www/device.js" name="device">
  14         <clobbers target="device" />
  15     </js-module>
  16 
  17     <!-- firefoxos -->
  18     <platform name="firefoxos">
  19         <config-file target="config.xml" parent="/*">
  20             <feature name="Device">
  21                 <param name="firefoxos-package" value="Device" />
  22             </feature>
  23         </config-file>                                         
  24         
  25         <js-module src="src/firefoxos/DeviceProxy.js" name="DeviceProxy">
  26             <runs />
  27         </js-module>
  28     </platform>
  29 
  30     <!-- android -->
  31     <platform name="android">
  32         <config-file target="res/xml/config.xml" parent="/*">
  33             <feature name="Device" >
  34                 <param name="android-package" value="org.apache.cordova.device.Device"/>
  35             </feature>
  36         </config-file>
  37 
  38         <source-file src="src/android/Device.java" target-dir="src/org/apache/cordova/device" />
  39     </platform>
  40 
  41     <!-- ios -->
  42     <platform name="ios">
  43         <config-file target="config.xml" parent="/*">
  44             <feature name="Device">
  45                 <param name="ios-package" value="CDVDevice"/>
  46             </feature>
  47         </config-file>
  48 
  49         <header-file src="src/ios/CDVDevice.h" />
  50         <source-file src="src/ios/CDVDevice.m" />
  51     </platform>
  52 
  53     <!-- blackberry10 -->
  54     <platform name="blackberry10">
  55         <source-file src="src/blackberry10/index.js" target-dir="Device" />
  56         <config-file target="www/config.xml" parent="/widget">
  57             <feature name="Device" value="Device"/>
  58         </config-file>
  59         <config-file target="www/config.xml" parent="/widget/rim:permissions">
  60             <rim:permit>read_device_identifying_information</rim:permit>
  61         </config-file>
  62     </platform>
  63 
  64     <!-- wp7 -->
  65     <platform name="wp7">
  66         <config-file target="config.xml" parent="/*">
  67             <feature name="Device">
  68                 <param name="wp-package" value="Device"/>
  69             </feature>
  70         </config-file>
  71 
  72         <config-file target="Properties/WMAppManifest.xml" parent="/Deployment/App/Capabilities">
  73             <Capability Name="ID_CAP_IDENTITY_DEVICE" />
  74         </config-file>
  75 
  76         <source-file src="src/wp/Device.cs" />
  77     </platform>
  78 
  79     <!-- wp8 -->
  80     <platform name="wp8">
  81         <config-file target="config.xml" parent="/*">
  82             <feature name="Device">
  83                 <param name="wp-package" value="Device"/>
  84             </feature>
  85         </config-file>
  86 
  87         <config-file target="Properties/WMAppManifest.xml" parent="/Deployment/App/Capabilities">
  88             <Capability Name="ID_CAP_IDENTITY_DEVICE" />
  89         </config-file>
  90 
  91         <source-file src="src/wp/Device.cs" />
  92     </platform>
  93 
  94     <!-- windows8 -->
  95     <platform name="windows8">
  96         <js-module src="src/windows8/DeviceProxy.js" name="DeviceProxy">
  97             <merges target="" />
  98         </js-module>
  99     </platform>
 100 
 101 </plugin>
