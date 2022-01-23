## Welcome to SBCBox

[SBCBox](https://github.com/benjamin-ti/sbcbox) is my Single Board Computer Code Box. A collection of code and docs used as a knowledge base for SBCs, in particular for 
- BeagleBone **(Black)**
- Raspberry _Pi_

### Example

Simple `GPIO toggle` for BeagleBone Black

```markdown
#!/bin/bash

echo "60" > /sys/class/gpio/export
echo "out" > /sys/class/gpio/gpio60/direction

while true
do
    echo 1 > /sys/class/gpio/gpio60/value
    sleep 1
    echo 0 > /sys/class/gpio/gpio60/value
    sleep 1
done
```
