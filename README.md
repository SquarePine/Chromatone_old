# SquarePine - Chromatone

---

## Get Started - After Forking & Forking

### Typical Update

#### First Download

Run the following git commands on the repository:

```bash
git submodule update --init --recursive
```

#### Any Other Update

Run the following git commands on the repository:

```bash
git submodule update --recursive
```

### Purging Submodules to Forcibly Update

If you're running into troubles updating your submodules, try cleaning up everything and removing the local submodule files first before reupdating them.

You may use the script below to faciliate this process:

```bash
git clean -dfx
git reset --hard
rm -rf submodules/AudioWorks*
git fetch --all
git rebase upstream/master
git submodule update --init --recursive
```

---

## How to Build the Application

* Open, build and run the Projucer project.
  * Found under `submodules/JUCE/extras/Projucer/Builds`.
* Open the `Sounite.jucer` file, hit save, and open the appropriate project for your IDE.

---

## Submodule Dependencies

### Internal

- https://github.com/SquarePine/SquarePineAudio
- https://github.com/SquarePine/SquarePineCore
- https://github.com/SquarePine/SquarePineGraphics
- https://github.com/SquarePine/SquarePineMaths

### Third Party

- https://github.com/WeAreROLI/JUCE
- https://github.com/dbry/WavPack
