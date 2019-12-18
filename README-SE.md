# No Health Reset

_No Health Reset_ is a mod for [The Elder Scrolls V: Skyrim][Skyrim] to revert
full health recovery, which occurs when the player sleeps and levels up.

It is intended to work with any mod which reduces or zeroes health
regeneration, such as [No Health Regen] or [Realistic Health Regeneration].

It can also be used to emulate a similar feature present in [Requiem] [until
version 2.0.2][#1], for instance if using a port to Special Edition, for which
the corresponding SKSE plugin was not converted, or a later release, in which
[the feature was removed][#1].


## Requirements

- [The Elder Scrolls V: Skyrim][Skyrim].

- [SKSE].

- A mod or tweak to decrease health regeneration, since vanilla rate wouldn't
  allow to appreciate the effects of this mod.

  Examples include, but are not limited to:

  - [No More Passive Health Regeneration];
  - [Realistic Regeneration - RealRegen];
  - [Requiem];
  - [SkyTweak];
  - using [modAV in console][Targeted Commands] to reduce _HealRate_;
  - directly modifying _Health Regen_ in the [Race] record.


## Installation

- Copy the ESP file and Scripts folder to Skyrim's Data folder, using [Mod
  Organizer 2] is recommended.


## Known Issues

- Health can be reduced to lower than the initial value, possibly causing
  death, when the resulting regeneration rate is below zero: for example this
  is the case when combining the effect of a mod above with the penalty for
  high exposure given by [Frostfall].

  Note that this is not consistent with how the game handles a negative value
  of regeneration, since it wouldn't cause additional health damage;
  nonetheless I left this side effect as an incentive for players to restore
  their condition before going to sleep.


[Skyrim]: https://elderscrolls.bethesda.net/skyrim
[SKSE]: https://skse.silverlock.org/
[No More Passive Health Regeneration]: https://www.nexusmods.com/skyrimspecialedition/mods/15447
[Realistic Regeneration - RealRegen]: https://www.nexusmods.com/skyrimspecialedition/mods/14437
[Requiem]: https://www.nexusmods.com/skyrim/mods/19281
[#1]: https://www.reddit.com/r/skyrimrequiem/comments/axou15/requiem_news_requiem_300_consign_to_oblivion_is/ehxmwai
[SkyTweak]: https://www.nexusmods.com/skyrim/mods/33395
[Targeted Commands]: https://en.uesp.net/wiki/Skyrim:Console#Targeted_Commands
[Race]: https://www.creationkit.com/index.php?title=Race
[Mod Organizer 2]: https://www.nexusmods.com/skyrimspecialedition/mods/6194
[Frostfall]: https://www.nexusmods.com/skyrim/mods/11163