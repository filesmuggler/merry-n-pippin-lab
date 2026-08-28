# Hardware

SO-101 kit source: [LeRobot SO-101](https://huggingface.co/docs/lerobot/so101). Vision is two views, not one camera asked to do everything: Brio on the table, FIT0701 on the gripper.

## BOM

| Item | Qty | Model / SKU | Spec | Role |
| --- | ---: | --- | --- | --- |
| Merry | 1 | SO-101 leader | — | Teleop leader |
| Pippin | 1 | SO-101 follower | — | Manipulation |
| Feetech STS3215 (1/345) | 7 | C001 | — | Follower joints + leader shoulder |
| Feetech STS3215 (1/191) | 2 | C044 | — | Leader base + elbow |
| Feetech STS3215 (1/147) | 3 | C046 | — | Leader wrist + gripper |
| Motor control board | 2 | Waveshare bus | — | One per arm |
| PSU | 2 | 5 V DC, kit spec | — | One per arm |
| USB-C cable | 2 | — | — | Arm ↔ workstation |
| Scene camera | 2 | [Logitech Brio 100](https://www.logitech.com/en-eu/products/webcams/brio-100-webcam.960-001585.html) (`960-001585`) | 1080p, 58.9° diag FOV, fixed | Table / external workspace |
| Camera stand | 1 | [NEEWER clamp stand](https://www.amazon.pl/NEEWER-regulowany-zaciskiem-lustrzanek-cyfrowych/dp/B0B8CM9DGG) (`B0B8CM9DGG`) | Clamp-mounted | Carries the Brios |
| Brio stand adapter | 2 | [Thingiverse 6929603](https://www.thingiverse.com/thing:6929603/files), modified | PETG | Brio → NEEWER stand |
| Wrist camera | 1 | [DFRobot FIT0701](https://www.digikey.pl/pl/products/detail/dfrobot/FIT0701/13166487) | USB 2.0, 640×480, 30 × 25 × 21.4 mm | Eye-in-hand on Pippin |
| Wrist camera mount | 1 | [SO-ARM101 hex-nut 32×32 UVC](https://github.com/TheRobotStudio/SO-ARM100/blob/main/Optional/SO101_Wrist_Cam_Hex-Nut_Mount_32x32_UVC_Module/stl/SO-ARM101_camera_wrist_mount.stl) | PETG | FIT0701 on Pippin wrist |
| Table clamp | 4 | — | — | Arms to desk |
| 3D-printed structure | 1 set | SO-101 STLs | PETG | Frames, gripper |
| Filament | — | [Prusament PETG](https://prusament.com/pl/materials/prusament-petg/), [ROSA3D PET-G](https://www.rosa3d.pl/filament/pet-g) | Printed on Prusa MINI+ | Camera adapters + wrist mount |
| Desk | 1 | [IKEA VIHALS](https://www.ikea.com/pl/pl/p/vihals-stol-bialy-bialy-s39578509/) (`395.785.09`) | White | Build station |
| Workstation | 1 | Consumer GPU, VRAM TBD | — | Teleop, train, infer |

Servo qty is one leader + one follower ([upstream kit](https://huggingface.co/docs/lerobot/so101)). Brio qty is a set of two for the table view — correct the row if the bench differs.
