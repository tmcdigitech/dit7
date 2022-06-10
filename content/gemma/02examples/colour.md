---
title: A flash of colour
weight: 30
---

```python
import adafruit_dotstar as dotstar
import board
import time

# One pixel connected internally!
dot = dotstar.DotStar(board.APA102_SCK, board.APA102_MOSI, 1, brightness=0.2)

while True:
  dot[0] = (255, 0, 0)
  time.sleep(0.5)
  dot[0] = (0, 255, 0)
  time.sleep(0.5)
  dot[0] = (0, 0, 255)
  time.sleep(0.5)
```
