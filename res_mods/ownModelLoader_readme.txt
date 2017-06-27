ownModel loader V1.363
	by atacms
	compatibility as of now v0.9.19.0.2
--------------------------------------------
A universal model loader originally designed to address the hitbox mismatch issue caused by using remodels significantly different from stock models.


--------------------------------------------
This mod has the option to change only the model of tanks controlled by player, leaving friendly and enemy tanks untouched.
It has the option to link a specific remodel to a designated list of tanks. 
It has the option to manage multiple remodel profiles and apply them individually or all at once.

This mod also provide base layer support for some advanced feature for remodels. It's not necessary to setup and enable 
a profile in ownModel.xml to use these advanced feature. Simply having this mod in res_mods folder will be sufficient.
Note that this is meant for remodel makers. ownModel loader provides the capability, it's up to the remodel itself to use these abilities.

These advaned features included but not limited to :
[*]animate multiple turrets and guns
[*]load different tank skin based on map type (summer, winter or desert)
[*]auto-rotate certain parts, like tank cooling fan.
[*]search animation. Rotate a component toward random direction, wait a few seconds then turn to a new random direction
[*]if a camouflage net is equipted, a camouflage net model will be attached to hull as soon as this equipment came into 
   effect (ie. idle for a few seconds). And will be removed as soon as the tank starts moving again.


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
V1.363
#fixed stuck at loading when certain tank is in the game(obj907A for example)
#fixed missing inscriptions if inscription layout is different between original and remodel
#known issue: in above case, clicking inscription slot in customization menu still cause inscriptions to vanish

V1.362
#fixed autorotor for old remodels(Leopard2A5)
#fixed broken customizations for Czech/Sweden tanks

V1.361
#fixed crash when using non-levered independent suspension without segmented track

V1.36
#added some new animation bones to be used in gun geometry. (instruction_on_new_animationBone.txt)
#these new bones receive a unique animator to perform varies tasks like autorotation or follow user viewpoint
#previous add-on model feature is to be replaced by these bones. Old mechanism will remain to support old remodels

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