---
-api-id: E:Windows.Gaming.Input.FlightStick.HeadsetDisconnected
-api-type: winrt event
---

<!-- Event syntax.
public event TypedEventHandler HeadsetDisconnected<IGameController, Headset>
-->

# Windows.Gaming.Input.FlightStick.HeadsetDisconnected

## -description

Signals when a headset is disconnected from the flight stick.

## -remarks

For more information on detecting, tracking, and using headsets, see [Headset](https://docs.microsoft.com/windows/uwp/gaming/headset).

## -see-also

* [Windows.Gaming.Input.IGameController](igamecontroller.md)
* [Windows.Gaming.Input.Headset](headset.md)

## -examples

The following example shows how to register a handler for this event. `flightStick` is a **FlightStick** that's connected to the device.

```cpp
flightStick.HeadsetDisconnected += ref new TypedEventHandler<IGameController^, Headset^>(
    [] (IGameController^ device, Headset^ headset)
{
    // Enable headset capture and playback on this device.
});
```