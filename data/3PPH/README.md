# 3PPH - Scenario B: Freely floating model

These files are the unfiltered measurements from the freely floating model tests. The sensors and their configuration are documented in the [experimental setup](../../docs/experimental_setup.md).

The files are named with the following naming convention`3PPH_Rep.csv` 

`PP` denotes the applied incident wave period/frequency, from the list below. `H` denotes wether $H_1 = 0.024$ m or $H_2 = 0.04$ m was applied.

As an example, `3071_2.csv` are the scenario B time series for
- `PP = 07` $\rightarrow T = 1.113 $
- `H=1` $\rightarrow H = 0.024$ m
- `_Rep=2` $\rightarrow$ This is the second repetition.

| Index | $\xi_B$ [-] | $\omega$ [rad/s] | $T$ [s]   | $k$ [rad/m] | $\lambda$ [m]  | $c_g$ [m/s] | $h/\lambda$ [-] | Refl. Time [s] | $\lambda / L_{Beach}$ [-] |
|------:|--------:|-----------:|--------:|-----------:|--------:|-----------:|----------:|----------------:|----------------:|
| 1     | 0.350   | 4.143      | 1.516   | 1.750     | 3.590   | 1.184     | 0.279    | 10.137          | 1.995          |
| 2     | 0.500   | 4.952      | 1.269   | 2.500     | 2.513   | 0.990     | 0.398    | 12.116          | 1.396          |
| 3     | 0.525   | 5.075      | 1.238   | 2.625     | 2.394   | 0.967     | 0.418    | 12.415          | 1.330          |
| 4     | 0.550   | 5.194      | 1.210   | 2.750     | 2.285   | 0.944     | 0.438    | 12.707          | 1.269          |
| 5     | 0.575   | 5.311      | 1.183   | 2.875     | 2.185   | 0.924     | 0.458    | 12.993          | 1.214          |
| 6     | 0.600   | 5.425      | 1.158   | 3.000     | 2.094   | 0.904     | 0.477    | 13.272          | 1.164          |
| 7     | 0.650   | 5.646      | 1.113   | 3.250     | 1.933   | 0.869     | 0.517    | 13.814          | 1.074          |
| 8     | 0.700   | 5.860      | 1.072   | 3.500     | 1.795   | 0.837     | 0.557    | 14.335          | 0.997          |
| 9     | 0.750   | 6.065      | 1.036   | 3.750     | 1.676   | 0.809     | 0.597    | 14.839          | 0.931          |
| 10    | 1.000   | 7.004      | 0.897   | 5.000     | 1.257   | 0.700     | 0.796    | 17.134          | 0.698          |
| 11    | 1.250   | 7.830      | 0.802   | 6.250     | 1.005   | 0.626     | 0.995    | 19.157          | 0.559          |
| 12    | 1.500   | 8.578      | 0.733   | 7.500     | 0.838   | 0.572     | 1.194    | 20.985          | 0.465          |
| 13    | 1.750   | 9.265      | 0.678   | 8.750     | 0.718   | 0.529     | 1.393    | 22.666          | 0.399          |
| 14    | 2.000   | 9.905      | 0.634   | 10.000    | 0.628   | 0.495     | 1.592    | 24.231          | 0.349          |

We have the data from 15 sensors in these tests
- `WM_Position [m]`: he horizontal stroke of the wave maker measured 1.5 m above the hinge.
- `WP_* [m]`: The surface elevation measured at wave probes `1`, `2`, `3`, `4`, and `6`
- `Sway/Heave/Roll [m]/[rad]`: The rigid body motions in the inertial reference frame measured by the visual markers.
- `Tension_* [N]`: The tension in the `_SB` (starboard) and `_PS` (port side) springs, as measured by the ring-type strain gauges.
- `Force_Sway [N]`: The shear forces is through the vertical rail in sway direction, as measured by the bending beam strain gauge.
- `ACC_* [m/s2]`: The body-fixed accelerations measured at `_HEAVE_SB` (vertical, starboard), `_HEAVE_PS` (vertical, port side), and `_SWAY` (horizontal, bottom) 


![Wave flume](../../docs/figures/The%20wave%20flume%20and%20wave%20probe%20positions.png)

The model in it's neutral position was position in the location of wave probe 5, $7$ m from the wave-maker.

![The freely floating model](../../docs/figures/Scenario%20B%20-%20The%20freely%20floating%20model.png)

> **Known error**: We had some issues with the innacurate time recordings from the camera tracking the visual markers. As a result, the rigid body motions in the inertial reference frame (sway, heave, roll) in these file can be slightly out of phase with the body motions measured by the accelerometers.