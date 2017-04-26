#### yolo2
This repository can evaluate darknent trained model on pytorch which loads darkent trained weight file directly. See test_tiny_yolo.py as an example.

#### Todo
- [x] load darknet weights to pytorch
- [x] evaluate tiny-yolo on single image
- [ ] evaluate face test data

#### Note
1. be sure to add m.eval()
2. running_var is processed differently
   - darkent: sqrt(running_var) + 0.00001
   - pytorch: sqrt(running_var + 0.00001)
