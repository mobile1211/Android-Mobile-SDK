<div class="article"><h1 ><font color="#AAA">class </font>Aircraft</h1></div>

~~~java
 class Aircraft extends BaseProduct 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.products</td></tr><tr valign="top"><td width=15%><font color="#999"><i>Inherits From:</i></td><td width=85%><font color="#999"><code><a href="/BaseClasses/DJIBaseProduct.html#djibaseproduct">BaseProduct</a></code></td></tr></table></html>



##### Description:



<font color="#666">Aircraft product class, which includes basic product information and access to all components (such as flight controller, battery etc.). This object is accessed from <code><a href="/Components/SDKManager/DJISDKManager.html#djisdkmanager_product">getProduct</a></code> in <code><a href="/Components/SDKManager/DJISDKManager.html#djisdkmanager">DJISDKManager</a></code>. 



##### Class Members:

<div class="api-row" id="djiaircraft_flightcontroller"><div class="api-col left">Components</div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djiaircraft_flightcontroller_inline">getFlightController</a></div></div><div class="inline-doc" id="djiaircraft_flightcontroller_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getFlightController</h6></div>

~~~java
 FlightController getFlightController() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.products</td></tr></table></html>



##### Description:



<font color="#666">Returns an instance of the aircraft's flight controller.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41"><a href="/Components/FlightController/DJIFlightController.html#djiflightcontroller">FlightController</a></td><td><font color="#666"><i>DJIFlightController component.</i></td></tr></table></html></div>

<div class="api-row" id="djiaircraft_cameras"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djiaircraft_cameras_inline">getCameras</a></div></div><div class="inline-doc" id="djiaircraft_cameras_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getCameras</h6></div>

~~~java
@Nullable
 synchronized List<Camera> getCameras() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr></table></html>



##### Description:



<font color="#666">Retrieves instances of the product's cameras. This is used when the aircraft has multiple DJI cameras, e.g. M210 and  M210 RTK. Note, when two cameras do exist, camera order within the array will not always the same. For example: On the  M210, the port side (left) camera will have an index of 0 and the starboard side (right)  camera will have an index of 1. However, the first object of <code><a href="/Products/Aircraft/DJIAircraft.html#djiaircraft_cameras">getCameras</a></code> will not  necessarily always be the camera with <code><a href="/Components/BaseComponent/DJIBaseComponent.html#djibasecomponent_index">getIndex</a></code> of 0.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41">synchronized List&lt;<a href="/Components/Camera/DJICamera.html#djicamera">Camera</a>&gt;</td><td><font color="#666"><i>A list of the aircraft's cameras.</i></td></tr></table></html></div>

<div class="api-row" id="djiaircraft_getcamerawithcomponentindex"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djiaircraft_getcamerawithcomponentindex_inline">getCameraWithComponentIndex</a></div></div><div class="inline-doc" id="djiaircraft_getcamerawithcomponentindex_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getCameraWithComponentIndex</h6></div>

~~~java
@Nullable
 Camera getCameraWithComponentIndex(int index) 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr></table></html>



##### Description:



<font color="#666">Retrieves an instance of the device's camera with inputted index.



##### Input Parameters:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41">int <font color="#000">index</td><td><font color="#666"><i>An int value.</i></td></tr></table></html>

##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41"><a href="/Components/Camera/DJICamera.html#djicamera">Camera</a></td><td><font color="#666"><i>An instance of the aircraft's camera.</i></td></tr></table></html></div>

<div class="api-row" id="djiaircraft_gimbals"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djiaircraft_gimbals_inline">getGimbals</a></div></div><div class="inline-doc" id="djiaircraft_gimbals_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getGimbals</h6></div>

~~~java
 synchronized List<Gimbal> getGimbals() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.products</td></tr></table></html>



##### Description:



<font color="#666">Retrieves instances of the product's gimbals. This is used when the aircraft has multiple DJI gimbals, e.g. M210  and M210 RTK. Note, when two gimbals do exist, gimbal order within the array will not always the same. For example:  On the M210, the port side (left) gimbal will have an index of 0 and the starboard  side (right) gimbal will have an index of 1. However, the first object of <code><a href="/Products/Aircraft/DJIAircraft.html#djiaircraft_gimbals">getGimbals</a></code>  will not necessarily always be the gimbal with <code><a href="/Components/BaseComponent/DJIBaseComponent.html#djibasecomponent_index">getIndex</a></code> of 0.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41">synchronized List&lt;<a href="/Components/Gimbal/DJIGimbal.html#djigimbal">Gimbal</a>&gt;</td><td><font color="#666"><i>A list of the aircraft's gimbals.</i></td></tr></table></html></div>

<div class="api-row" id="djiaircraft_remotecontroller"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djiaircraft_remotecontroller_inline">getRemoteController</a></div></div><div class="inline-doc" id="djiaircraft_remotecontroller_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getRemoteController</h6></div>

~~~java
 RemoteController getRemoteController() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.products</td></tr></table></html>



##### Description:



<font color="#666">Returns an instance of the aircraft's remote controller.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41"><a href="/Components/RemoteController/DJIRemoteController.html#djiremotecontroller">RemoteController</a></td><td><font color="#666"><i>DJIRemoteController component.</i></td></tr></table></html></div>

<div class="api-row" id="djiaircraft_mobileremotecontroller"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djiaircraft_mobileremotecontroller_inline">getMobileRemoteController</a></div></div><div class="inline-doc" id="djiaircraft_mobileremotecontroller_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getMobileRemoteController</h6></div>

~~~java
 MobileRemoteController getMobileRemoteController() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.products</td></tr></table></html>



##### Description:



<font color="#666">A simulated remote controller on the mobile device. It is supported by Mavic Pro and Spark using WiFi.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41"><a href="/Components/MobileRemoteController/DJIMobileRemoteController.html#djimobileremotecontroller">MobileRemoteController</a></td><td><font color="#666"><i>DJIMobileRemoteController component.</i></td></tr></table></html></div>

<div class="api-row" id="djiaircraft_basestation"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djiaircraft_basestation_inline">getBaseStation</a></div></div><div class="inline-doc" id="djiaircraft_basestation_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getBaseStation</h6></div>

~~~java
 BaseStation getBaseStation() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.products</td></tr></table></html>



##### Description:



<font color="#666">The connected base station instance. It is supported by Phantom 4 RTK and Matrice 210 RTK V2.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41"><a href="/Components/RTKBaseStation/DJIRTKBaseStation.html#djirtkbasestation">BaseStation</a></td><td><font color="#666"><i>An instance of <code><a href="/Components/RTKBaseStation/DJIRTKBaseStation.html#djirtkbasestation">BaseStation</a></code>.</i></td></tr></table></html></div>



##### Inherited Methods:

<div class="api-row" id="djibaseproduct_setupdatediagnosticslistcallback"><div class="api-col left">dji.sdk.base.BaseProduct</div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djibaseproduct_setupdatediagnosticslistcallback_inline">setDiagnosticsInformationCallback</a></div></div><div class="inline-doc" id="djibaseproduct_setupdatediagnosticslistcallback_inline"

><div class="article"><h6 ><font color="#AAA">method </font>setDiagnosticsInformationCallback</h6></div>

~~~java
 void setDiagnosticsInformationCallback(DiagnosticsInformationCallback callback) 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr></table></html>



##### Description:



<font color="#666">Sets up the diagnostics list update callback.



##### Input Parameters:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41"><a href="/Components/Diagnostics/DJIDiagnostics_DiagnosticsInformationCallbackInterface.html#djidiagnostics_diagnosticsinformationcallbackinterface">DiagnosticsInformationCallback</a> <font color="#000">callback</td><td><font color="#666"><i>The callback of <code><a href="/Components/Diagnostics/DJIDiagnostics_DiagnosticsInformationCallbackInterface.html#djidiagnostics_diagnosticsinformationcallbackinterface">DiagnosticsInformationCallback</a></code>.</i></td></tr></table></html></div>

<div class="api-row" id="djibaseproduct_getfirmwarepackageversion"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djibaseproduct_getfirmwarepackageversion_inline">getFirmwarePackageVersion</a></div></div><div class="inline-doc" id="djibaseproduct_getfirmwarepackageversion_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getFirmwarePackageVersion</h6></div>

~~~java
 String getFirmwarePackageVersion() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr><tr valign="top"><td width=15%><font color="#999"><i>SDK Key:</i></td><td width=85%><font color="#999"><a href="/Components/KeyManager/DJIProductKey.html#productkey_firmware_package_version_key">ProductKey.FIRMWARE_PACKAGE_VERSION</a></td></tr></table></html>



##### Description:



<font color="#666">Gets the product's firmware package version. Products other than Phantom 4, Phantom 4 Pro, Mavic Pro, and Inspire 2, require internet connection. The execution time for this method depends on the speed of internet connectivity.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41">String</td><td><font color="#666"><i>The product's firmware package version string.</i></td></tr></table></html></div>

<div class="api-row" id="djibaseproduct_setname"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djibaseproduct_setname_inline">setName</a></div></div><div class="inline-doc" id="djibaseproduct_setname_inline"

><div class="article"><h6 ><font color="#AAA">method </font>setName</h6></div>

~~~java
 void setName(@NonNull String name, @Nullable final CommonCallbacks.CompletionCallback callback)
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr></table></html>



##### Description:



<font color="#666">Retrieves the model of the product.



##### Input Parameters:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41">@NonNull String <font color="#000">name</td><td><font color="#666"><i>Name to be set to the aircraft.</i></td></tr><tr valign="top"><td><font color="#70BF41">@Nullable final <a href="/Utils/DJICommonCallbacks.html#djicommoncallbacks">CommonCallbacks</a>.CompletionCallback <font color="#000">callback</td><td><font color="#666"><i>Asynchronous execution result.</i></td></tr></table></html></div>

<div class="api-row" id="djibaseproduct_getname"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djibaseproduct_getname_inline">getName</a></div></div><div class="inline-doc" id="djibaseproduct_getname_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getName</h6></div>

~~~java
 void getName(final CommonCallbacks.CompletionCallbackWith<String> callback)
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr></table></html>



##### Description:



<font color="#666">Retrieves the model of the product.



##### Input Parameters:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41">final <a href="/Utils/DJICommonCallbacks.html#djicommoncallbacks">CommonCallbacks</a>.CompletionCallbackWith&lt;String&gt; <font color="#000">callback</td><td><font color="#666"><i>The execution callback with the returned value.</i></td></tr></table></html></div>

<div class="api-row" id="djibaseproduct_model"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djibaseproduct_model_inline">getModel</a></div></div><div class="inline-doc" id="djibaseproduct_model_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getModel</h6></div>

~~~java
 Model getModel() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr><tr valign="top"><td width=15%><font color="#999"><i>SDK Key:</i></td><td width=85%><font color="#999"><a href="/Components/KeyManager/DJIProductKey.html#productkey_model_name_key">ProductKey.MODEL_NAME</a></td></tr></table></html>



##### Description:



<font color="#666">Retrieves the model of the product. See <code><a href="/Products/Aircraft/DJIAircraft.html#djiaircraft">Aircraft</a></code> and <code><a href="/Products/Handheld/DJIHandheld.html#djihandheld">HandHeld</a></code> for the possible strings that can be returned.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41"><a href="/BaseClasses/DJIBaseProduct.html#djimodelnamestring">Model</a></td><td><font color="#666"><i>The model of the product.</i></td></tr></table></html></div>

<div class="api-row" id="djibaseproduct_connected"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djibaseproduct_connected_inline">isConnected</a></div></div><div class="inline-doc" id="djibaseproduct_connected_inline"

><div class="article"><h6 ><font color="#AAA">method </font>isConnected</h6></div>

~~~java
 boolean isConnected() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr><tr valign="top"><td width=15%><font color="#999"><i>SDK Key:</i></td><td width=85%><font color="#999"><a href="/Components/KeyManager/DJIProductKey.html#productkey_connection_key">ProductKey.CONNECTION</a></td></tr></table></html>



##### Description:



<font color="#666"><code>true</code> if the device is connected.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41">boolean</td><td><font color="#666"><i><code>true</code> if the device is connected.</i></td></tr></table></html></div>

<div class="api-row" id="djibaseproduct_getcamera"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djibaseproduct_getcamera_inline">getCamera</a></div></div><div class="inline-doc" id="djibaseproduct_getcamera_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getCamera</h6></div>

~~~java
 Camera getCamera() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr></table></html>



##### Description:



<font color="#666">Retrieves an instance of the device's camera. Only supported by the product with single gimbal, except Zenmuse XT2 and Mavic 2 Enterprise Camera.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41"><a href="/Components/Camera/DJICamera.html#djicamera">Camera</a></td><td><font color="#666"><i>An instance of the aircraft's camera.</i></td></tr></table></html></div>

<div class="api-row" id="djibaseproduct_getbattery"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djibaseproduct_getbattery_inline">getBattery</a></div></div><div class="inline-doc" id="djibaseproduct_getbattery_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getBattery</h6></div>

~~~java
 Battery getBattery() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr></table></html>



##### Description:



<font color="#666">Retrieves an instance of the product's smart battery. When using products with multiple batteries, such as the M600 or Inspire 2, use <code><a href="/BaseClasses/DJIBaseProduct.html#djibaseproduct_getbatteries">getBatteries</a></code>, as this method will only return a single battery.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41">Battery</td><td><font color="#666"><i>An instance of the aircraft's smart battery.</i></td></tr></table></html></div>

<div class="api-row" id="djibaseproduct_getbatteries"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djibaseproduct_getbatteries_inline">getBatteries</a></div></div><div class="inline-doc" id="djibaseproduct_getbatteries_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getBatteries</h6></div>

~~~java
 synchronized List<Battery> getBatteries() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr></table></html>



##### Description:



<font color="#666">Returns an array of aircraft's batteries. It is used when the aircraft has multiple batteries, e.g. Matrice 600.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41">synchronized List&lt;Battery&gt;</td><td><font color="#666"><i>A List of <code><a href="/Components/Battery/DJIBattery.html#djibattery">Battery</a></code> objects.</i></td></tr></table></html></div>

<div class="api-row" id="djibaseproduct_getgimbal"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djibaseproduct_getgimbal_inline">getGimbal</a></div></div><div class="inline-doc" id="djibaseproduct_getgimbal_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getGimbal</h6></div>

~~~java
 Gimbal getGimbal() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr></table></html>



##### Description:



<font color="#666">Retrieves an instance of the device's gimbal.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41"><a href="/Components/Gimbal/DJIGimbal.html#djigimbal">Gimbal</a></td><td><font color="#666"><i>An instance of the aircraft's gimbal.</i></td></tr></table></html></div>

<div class="api-row" id="djibaseproduct_getairlink"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djibaseproduct_getairlink_inline">getAirLink</a></div></div><div class="inline-doc" id="djibaseproduct_getairlink_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getAirLink</h6></div>

~~~java
 AirLink getAirLink() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr></table></html>



##### Description:



<font color="#666">Retrieves an instance of the device's AirLink.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41"><a href="/Components/AirLink/DJIAirLink.html#djiairlink">AirLink</a></td><td><font color="#666"><i>An instance of the aircraft's AirLink.</i></td></tr></table></html></div>

<div class="api-row" id="djibaseproduct_getaccessoryaggregation"><div class="api-col left"></div><div class="api-col middle" style="color:#AAA">method</div><div class="api-col right"><a class="trigger" href="#djibaseproduct_getaccessoryaggregation_inline">getAccessoryAggregation</a></div></div><div class="inline-doc" id="djibaseproduct_getaccessoryaggregation_inline"

><div class="article"><h6 ><font color="#AAA">method </font>getAccessoryAggregation</h6></div>

~~~java
@Nullable
 AccessoryAggregation getAccessoryAggregation() 
~~~

<html><table class="table-supportedby"><tr valign="top"><td width=15%><font color="#999"><i>Package:</i></td><td width=85%><font color="#999">dji.sdk.base</td></tr></table></html>



##### Description:



<font color="#666">Retrieves an instance of the accessory aggregation.



##### Return:

<html><table class="table-inline-parameters"><tr valign="top"><td><font color="#70BF41"><a href="/Components/AccessoryAggregation/DJIAccessoryAggregation.html#djiaccessoryaggregation">AccessoryAggregation</a></td><td><font color="#666"><i>'NULL' if the product does not support accessories (e.g. spotlight, speaker or beacon).</i></td></tr></table></html></div>


