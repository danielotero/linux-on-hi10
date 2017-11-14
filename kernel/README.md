### Backlight workaround
To enable backlight control set at least this options:

```
CONFIG_PWM=y
CONFIG_PWM_CRC=y
CONFIG_I2C_DESIGNWARE_PLATFORM=y
CONFIG_I2C_DESIGNWARE_PCI=y
CONFIG_INTEL_SOC_PMIC=y
CONFIG_DRM_I915=m

CONFIG_PWM_LPSS=m
CONFIG_PWM_LPSS_PCI=m
CONFIG_PWM_LPSS_PLATFORM=m
```

The bug is tracked [here](https://bugs.freedesktop.org/show_bug.cgi?id=96571).

### Hardware buttons
To enable hardware keys set:

`CONFIG_SPI_DESIGNWARE=m`
