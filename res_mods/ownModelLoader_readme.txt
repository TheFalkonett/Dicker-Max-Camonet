ownModel loader V1.351
	by atacms
	compatibility as of now v0.9.18.0/0.9.19CT
--------------------------------------------
A universal model loader originally designed to address the hitbox mismatch issue caused by using remodels significantly different from stock models.


--------------------------------------------
This mod has the option to change only the model of tanks controlled by player, leaving friendly and enemy tanks untouched.
It has the option to link a specific remodel to a designated list of tanks. 
It has the option to manage multiple remodel profiles and apply them individually or all at once.


[Known Issues]
Resolved.

[Configuration]
mod config file <scripts/client/mods/ownModel.xml> is fully commented.


[Notes]
Current ownModel.xml contains profiles for the collection of stand-alone remodels. All of them are disabled by default.
You need to install corresponding model pack before activating them.
Unless the profile belongs to a stock WoT model in which case you can activate it directly.


--------------------------------------------
[Changelog]
V1.351
#WoT 0.9.19CT compatible

V1.35
#added support for <fixedInscription>, <fixedEmblem>
#added option to define recoil parameter, especially recoil length <amplitude>
#national inscriptions can now be invoked by any nation via <fixedInscription>
#these inscriptions in global domain have different ID format as explained at the beginning of ownModel.xml

V1.343
#minor fix for hull net model

V1.342
#fixed bug in loading seasonal model from outside ownModel profiles

V1.341
#added option to load different segmented tracks depending on map type (summer/desert/winter)

V1.34
#added option to load different model depending on map type (summer/desert/winter)

V1.33
#fixed profiles disabled via configReload is still active during gameplay

V1.32
#adapt to wot0.9.17.1

V1.31
#max mini-turret count increased to 8
#mini-turret can be mounted ontop main turret

V1.3
#added mini turret support (up to 2 mini-turrets)
#fixed hangar refresh cause CTD
#fixed exhaust effects for hull-aiming tanks.

V1.294
#fixed exhaust effect handling
#added levered suspension support
#added slave joints for gun animation bones
#added optional engine sound definition

V1.293
#stability improvements
#option to hide clan logo
#support random search animation for rotator addon.
#added hotkey 'F5' to reload config file in hangar.

V1.292
#adapt to wot0.9.16

V1.291
#improved hangar support for new attachments

V1.29
#added option to specify national emblems on tank models
#added option to define additional elevation(HP_acc_0) and auto-rotation(HP_acc_E0) node in turret visual file
#if such nodes are detected, acc_0.model and/or acc_E0.model will be attached to this node if found under the same folder

V1.28
#fixed crash when used on tanks with multiple hull variants (tiger1, caernarvon, conqueror, etc.)
#added optional hangarShadowTexture support

V1.27
#added hangar support
#added option to turn off hangar support 
#coding structure overhaul

V1.26
#adapt to wot0.9.15
#added gun Firing effect and reload sound support
#modified common lib copy_reg.py to suppress PyDirectParticleAttachment problem
#Fixed custom effect hardpoint problem, probably

V1.25
#adapt to wot0.9.12
#added full nationality emblems and inscriptions support
#cfg file is not fully up-to-date

V1.24
#fixed gun insignia support
#fixed AODecal checking condition
#disabled emblems and inscriptions

v1.23
#adapt to wot0.9.9, added chassis<AODecals> support

V1.22
#adapt to wot0.9.8
#all cfg entry updated for wot0.9.8

V1.21
#adapt to wot0.9.7

V1.2
#adapt to wot0.9.6
#clean up python.log dump

V1.1
#added destroyed model support
#added gun insignia support
#changed config filename from .cfg to .xml

V1.0
#Initial release