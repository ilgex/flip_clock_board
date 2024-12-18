# *Flip Clock*

FlipClock will default to Theme colors but can be further customized through constructor parameters.

The default flip direction is AxisDirection.down and the default animation curve is a custom curve that acceletares like gravity and bounces back at the end (like a mechanical bang).

In the example below some colors are inherited by a parent ThemeData from the amber color scheme. While some colors are defined in the constructor invocation:

<img src="https://raw.githubusercontent.com/ilgex/flip_clock_board/master/assets/flip_clock_board.gif?raw=true" width="299" height="126"  />

```dart
  Widget _flipClock(ColorScheme colors) =>
    Container(
      decoration: BoxDecoration(
        color: colors.onPrimary,
        borderRadius: const BorderRadius.all(Radius.circular(8.0)),
      ),
      padding: const EdgeInsets.all(16.0),
      child: FlipClock(
        digitSize: 54.0,
        width: 46.0,
        height: 62.0,
        separatorColor: colors.primary,
        hingeColor: Colors.black,
        showBorder: true,
      ),
    );
```