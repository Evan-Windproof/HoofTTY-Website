# HoofTTY Official Website

HoofTTY is an experimental pony-themed text-mode operating system.

- **Official website:** https://hooftty.evanwindproof.top/
- **Main project hub:** https://evanwindproof.top/projects/hooftty/
- **Operating system source and releases:** https://github.com/Evan-Windproof/HoofTTY

This repository contains a deployable mirror of the HoofTTY website page from the main Evan Windproof website. The authoritative page source remains in [Evan-Windproof.github.io](https://github.com/Evan-Windproof/Evan-Windproof.github.io/tree/main/projects/hooftty).

The mirror is published independently through GitHub Actions and GitHub Pages. The workflow copies only `projects/hooftty/` into the Pages artifact and includes the root `CNAME` file. Repository documentation and other management files are not published as website content.

## Updating the website

Make website changes in the main website repository first. The main website's **Sync HoofTTY website mirror** workflow copies the authoritative page into this repository and records the source commit in `.hooftty-source`. A push that updates `projects/hooftty/` triggers the deployment workflow.

Avoid editing the mirrored page directly unless you are performing a reviewed recovery or deployment fix. See the [main website synchronization guide](https://github.com/Evan-Windproof/Evan-Windproof.github.io/blob/main/docs/HOOFTTY.md) for the synchronization procedure.

## Local preview

Run the following from this repository root:

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000/projects/hooftty/.

## Website assets

The original Evan pixel sprite comes from the [HoofTTY Beta 0.4.0 source](https://github.com/Evan-Windproof/HoofTTY/blob/beta0.4.0/include/Pony/evan.h). The Silkscreen font is available under the [SIL Open Font License](projects/hooftty/silkscreen-OFL.txt).
