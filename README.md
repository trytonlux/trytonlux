# <span style="color: #ff5555;">𝝺</span> Tryton Van Meer

```python
#!/usr/bin/env python3
import Developer from persons.developer
import Desktop from computers.desktop
import Laptop from computers.laptop

if __name__ == "__main__":
    desktop = Desktop(
        hostname="caffeine-pc"
        cpu="AMD Ryzen 5 2600",
        cpu_cooler="be quiet! Dark Rock Pro 4",
        motherboard="MSI B350 TOMAHAWK",
        ram="G.Skill Trident Z RGB (2x8GB)",
        gpu="Sapphire Radeon RX 5700XT NITRO+",
        case="Fractal Design Meshify S2",
        psu="Corsair RMx 750W",
        mouse="Logitech G703 LIGHTSPEED",
        keyboard="Massdrop x MiTo Laser ALT",
        microphone="Audio-Technica AT2020USB+"
    )

    tryton = Developer(
        name="Tryton",
        os=["Arch Linux", "Fedora"],
        desktop="GNOME",
        editor="VSCode",
        terminal="Tilix",
        shell="Fish",
        font="JetBrains Mono",
        colors="Dracula",
        computers=[desktop, laptop(model="Surface Pro 3", hostname="silver-pc")]
    )

    while True:
        try:
            tryton.consume_caffeine()
            tryton.code()
        except KeyboardInterrupt:
            tryton.sleep()
            break
```