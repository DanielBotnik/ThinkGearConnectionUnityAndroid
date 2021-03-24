# ThinkGearConnectionUnityAndroid
Interface for connecting Unity with ThinkGear For Android.

# How to use
Drag the ThinkGear prefab from Project view to Hierarchy view in order to use it.

```
  ThinkGear thinkGear = GameObject.Find("ThinkGear").GetComponent<ThinkGear>();
  thinkGear.UpdateConnectedStateEvent += OnConnectFunction;
  thinkGear.UpdateMeditationEvent += CheckMeditationFunction;
```
And there are a lot more events that can be used not only the ones in the example.

In order to start monitoring use
```
  thinkGear.startMonitoring();
```
but if the device is not connected yet, it wont work.
