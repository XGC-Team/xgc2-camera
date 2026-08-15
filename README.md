# xgc2-camera

Public XGC-Team camera product. Every physical camera lives here. Vehicle
repos only assemble a launch; they do not vendor another capture stack.

| Path | Repository | Role |
| --- | --- | --- |
| `camera-core` | [xgc2-camera-core](https://github.com/XGC-Team/xgc2-camera-core) | ROS-independent V4L2 capture library |
| `camera-driver` | [xgc2-camera-driver](https://github.com/XGC-Team/xgc2-camera-driver) | ROS 1 V4L2 / USB / FS150 driver |
| `d435` | [xgc2-camera-d435](https://github.com/XGC-Team/xgc2-camera-d435) | D435 / D435i assembly (Scout and lab) |

`camera-driver/d435` is the same `xgc2-camera-d435` checkout, nested under
the ROS driver so USB and RealSense stay one camera family.

Clone recursively:

```bash
git clone --recurse-submodules git@github.com:XGC-Team/xgc2-camera.git
```
