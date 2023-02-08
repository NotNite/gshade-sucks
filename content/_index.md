+++
template = "index.html"
+++

# GShade Sucks

<subtitle>
  Resources for migrating from the aftermath of GShade
</subtitle>

## Resources

- [Guide to migrating from GShade to ReShade][guide]
- [GShade shader backup](https://kagamine.tech/shade/gshade.zip)
- [ReShade website (download links & Discord)][reshade]
- [GShade update patcher][patcher]

## What happened?

On February 6th, 2023, an update to GShade's installer was silently released that contained [malicious code](https://twitter.com/NotNite/status/1622597424589029376). This malicious code would shut off the user's PC when it detected the installer was being run in unauthorized ways.

Marot, the developer of GShade, [admitted that this was purposefully done](https://twitter.com/NotNite/status/1622623953838649344), and has said "anything could have been in the payload".

## What now?

Switch to [ReShade][reshade]. There is [a guide][guide] on how to migrate from GShade to ReShade.

ReShade is free, open source software, and reports indicate it performs faster than GShade (especially on low-end hardware).

## But I can keep using GShade if I want, right?

Not without modification. The developer of GShade was [banned off of GitHub](https://twitter.com/Tr3ntu/status/1622948121037742081). Given GShade's DRM requiring it to fetch information from GitHub before running, this means that GShade is now unusable.

If you *absolutely* need to use GShade, you can use [this patcher][patcher] to remove the update check. It is highly suggested you move to ReShade when you are ready to.

## Is it safe to use GShade with the patcher?

The malware in GShade was specifically inside of the installer code. Given that the installer is now non-functional, it is believed safe to use. It is still recommended to switch to ReShade.

## ReShade doesn't work as well as GShade!

Please report incompatibilities to the [Rika's Shader Porting Project][shader-porting-project] Discord server.

---

<footer>
  Support what we care about!
  <div class="footer-content">
    <a href="https://sfconservancy.org/">Support the Software Freedom Conservancy</a>
    <a href="https://www.eff.org/">Support the Electronic Frontier Foundation</a>
    Donate to your local animal shelter
  </div>
</footer>

[reshade]: <https://reshade.me/>
[guide]: <https://gist.github.com/ry00001/3e2e63b986cb0c673645ea42ffafcc26>
[patcher]: <https://notnite.com/gshade-patcher.html>
[shader-porting-project]: <https://discord.gg/9kQTCB5Xwh>
