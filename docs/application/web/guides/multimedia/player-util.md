# Audio Latency

You can control the audio latency mode of the W3C player.

This feature is supported in mobile and wearable applications only.

The main features of the Player Util API include the following:

- Getting the latency mode

  You can [get the current latency mode of the player](#getting-the-current-latency-mode) with the `getLatencyMode()` method.

- Setting the latency mode

  You can [set the latency mode of the player](#setting-the-latency-mode) with the `setLatencyMode()` method.

## Get the current latency mode

To get the current latency mode, use the `getLatencyMode()` method:

```
var latencyMode;
try {
    latencyMode = tizen.playerutil.getLatencyMode();
} catch (error) {
    console.log(error.name + ': ' + error.message);
}
```

## Set the latency mode

To set a new latency mode, use one of the available modes defined in the `LatencyMode` enumerator (in [mobile](../../api/latest/device_api/mobile/tizen/playerutil.html#LatencyMode) and [wearable](../../api/latest/device_api/wearable/tizen/playerutil.html#LatencyMode) applications):

```
try {
    tizen.playerutil.setLatencyMode('HIGH');
} catch (error) {
    console.log(error.name + ': ' + error.message);
}
```

## Related information
* Dependencies
  - Tizen 2.4 and Higher for Mobile
  - Tizen 2.3.1 and Higher for Wearable
* API References
  - [Mobile](../../api/latest/device_api/mobile/tizen/playerutil.html)
  - [Wearable](../../api/latest/device_api/wearable/tizen/playerutil.html)
