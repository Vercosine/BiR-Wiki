# Turbine design guide (by Vercosine)

I recommend doing this in a creative world, so you can easily test out your setup. (You can use the Fluid White Hole added by Phosphophyllite for an endless steam source.)

Make sure to read the general [Turbines](/biggerreactors/turbine.md) page so you can get an idea on how the turbines work, as I will focus only on the most important in the following.

## Estimating the rough size
My numbers may not be too right in place, but that's because this is estimation, so do try different turbine sizes than the ones suggested here.

- Small reactors <6B steam per tick
  - 3x3 internal turbine base (face with bearing) (exclude turbine walls)
  - max 3 layers of coils (always use `3x3` coil rings, larger are generally a waste of resources because they have diminishing effect)
  - 2x blade layers than coil layers

- Medium to mid-large reactors <30B steam per tick
  - 5x5 internal turbine base
  - max 7 layers of coils
  - 2x to 3x blade layers

- Larger reactors
  - Bigger™ Turbine

**Note**: There is a hard steam limit that depends on the area of the base. I haven't run into this yet, but if you do, just size up your base.

## Adjusting the build
If you're in a creative world and you are using an endless steam source to supply your turbine, use the built-in steam limiter in the turbine to control intake. Otherwise you can already connect the turbine to your reactor and change the steam output of the reactor using the control rods. In this case, set your turbine steam limiter high enough so that it doesn't interfere.\[1\]

Now it's time to adjust. You want the speed to be either around **900-1000 RPM** or **1800-1900 RPM** and the rotor efficiency in the UI to be **100%**.

Pick your RPM range. The difference is mostly linear, i.e. 1800 produces approx. double power and consumes approx. double steam, however 900 RPM may be more efficient overall (not proven).

To increase rotor efficiency, just add more blades. Make your turbine longer to accommodate more blades if you need them. If your rotor efficiency already skyrockets to 100% before reaching your targeted RPM, then get rid of some blades, as they add extra mass and increase steam requirements for no benefit. If you end up using many layers of blades (like over 30), then you should make your base bigger and redo this process.

If you're not inside the RPM ranges specified, or your turbine is using too much or too little steam than your liking, try to remove or add coil blocks to ease up or tense the drag on the rotor, then adjust rotor efficiency again. Rule of thumb: Number of coil blocks is approximately proportional to steam consumed.

**Note**: It is not necessary for blades or coils to be symmetric, you can place them however you like. See the main turbine page for further conditions.

## Fine-tuning
Your turbine should be in the RPM ranges specified, has 100% rotor efficiency on stable operation and is using approximately as much steam as your reactor is producing. Connect the turbine to your reactor if you haven't already.

Adjust all control rods (holding `alt`) by one percent up or down and quickly look at the changes in power production by the turbine. You want to get it as close as possible to the max power possible. Once changing control rods either up or down leads to less power, you can go ahead and adjust single control rods to taste. That's it!

**Note**: Despite the fact that the popup says the turbine is most optimal at 900 or 1800 RPM, the optimal point usually lies between **900-1000 and 1800-1900 RPM**, depending on design.

---

**Footnotes**:
\[1\] If you use the steam limiter, your turbine may use less steam than the reactor is supplying, causing the reactor exhaust tank to clog up. Once this happens, the reactor will stop continously boiling water and will quickly overheat. This will not lead to a meltdown but to a much worsened fuel economy. Make sure to not fill up the turbine exhaust tank either, as this will lead to the turbine processing less or no steam, thus slowing down or stopping, and causing the same to the reactor.