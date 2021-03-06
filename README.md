#HGR Community Fixes

*Home-Grown Fixes for Home-Grown Rockets.*

![HGR Community Fixes logo](https://github.com/Kerbas-ad-astra/HGR-Community-Fixes/raw/master/HGR%20Community%20Fixes%20logo.png)

##Features

I've been singing the praises of OrionKermin's Home Grown Rockets for a long time.  The jump from Size 1 to Size 2 parts is extremely steep -- a fourfold increase in thrust and an eightfold increase in mass.  Having a set of intermediate 1.875m parts and 2-seater command pods really helps smooth things out.  Unfortunately, Orion hasn't logged on since October 2015, so HGR hasn't kept up with the changes in the latter half of the 1.0.x releases, and there are also a few minor errors that haven't been corrected.  There are a couple of mods with 1.875m parts, but neither one is quite enough to substitute for HGR, so I and others have been sharing Module Manager patches to repair or improve various parts.  These patches were scattered about the latter pages of the HGR thread, but now they're all in one place.

The following patches are contained in this package (broken out into separate files so others can tinker and critque more easily):

* Class-0 antennas added to all pods, and the OX-SJ solar panel is a stackable class-1 antenna.
	* There's also a patch to remove the obsolete "powerCurve" from the solar panel.  It's probably harmless, but why risk it?
* Cost and mass fixes for the fuel tanks and fairing.
* Center of Pressure and Lift offsets for "descent" modules (the Type 45 Soy-Juice descent modules, the Lima, the Radish, and the Spud) and the heat shield, so capsules are passively aerodynamically stable.  Also, buoyancy parameters which match the stock capsules.
* The docking port is now surface-attachable.
* An engine patch to bring the engines' thermal properties in line with stock.
* Fairing patches to rebalance fairing masses.
* INTERNAL patches to reduce grumbling from KSP when RPM is not installed.
* A "KAS" patch to remove deprecated KASModuleGrabs from RCS thrusters and the solar panels.
* ModuleScienceLab is added to the Leek and Advanced Onion pods, so they can reset experiments and otherwise behave correctly.  Probes and labs also provide the appropriate KerbNet access and experiment storage capability (the Lima descent capsule can gather experiments internally, to carry them back home).
* A new "Garlic" supply pod, to supplement the Lima.  If you have KIS, it will have some "dry inventory" space.
	* If you have a life support addon installed (ECLSS, IFILS, Ioncross, Snacks!, TAC-LS, or USI-LS), the Garlic, Daikon, and Edamame service modules will include some extra supplies.
	* Even if you don't have those mods, the Garlic pod has SAS level 3, to help with docking.
* The 1.25m inline parachute is not surface-attachable, and now does not claim to be in the editor.  The 0.625m inline parachute now opens at the same altitudes and pressures as the Mk16.
* The RCS parts have the new plume and sound effects.
* A fully-staffed Pumpkin pod or suitably-staffed Leek laboratory can be used to provide control of probes.  (With one hop.)
* Engine patches for the SoyJuice descent modules and service module.  The descent modules now have Isp curves like Sepratrons, and their TWRs match.  If you have the latest version of Landertron (0.11+), the engines can be set to automatically fire just before landing, just like the Soyuz.  If BahamutoD's Animated Engines or Nertea's Deployable Engines is installed, the Edamame service module's engine cover will automatically respond to the activation and deactivation of the engine.
* Tags for the stock searching system and constraints for part tests.
* Tech tree adjustments, both for stock and Community Tech Tree.
* A texture-name-fixing patch for the Radish decoupler.
* Thermal updates so that the capsules match stock capsules, and so that the discrete heat shield, the Radish, and the Spud match stock heat shields.  (They also properly support the 1.0.x updates for Deadly Reentry, I think.)
* WindowShine reflections for the solar panels (sadly, getting shiny windows requires modifications to the textures themselves, which is not happening until Orion comes back).
* A "backup" RPM config, in case people forget (or rather, so that people aren't forced to remember) to change HGR/Spaces/SoyInt/internal2_RPM**.txt** to a **.cfg** file.

##Dependencies

HGR Community Fixes depends on [**Home Grown Rockets**](http://forum.kerbalspaceprogram.com/index.php?/topic/55521-102hgr-1875m-partsv130-released/) (v1.3.0), of course, and [**Module Manager**](http://forum.kerbalspaceprogram.com/index.php?/topic/50533-105-module-manager-2618-january-17th-with-even-more-sha-and-less-bug/).

##Recommended addons

If you're going to use 1.875m parts, you might as well get [**Filter Extension**](http://forum.kerbalspaceprogram.com/index.php?/topic/93955-105-filter-extensions-2412-nov-10/) so that the "size1p5" category gets a proper icon and description in the "Filter by Cross-Section" menu.

##Suggested addons

Crawling through the part configs and weeding out years' worth of accumulated cruft got me thinking about alternatives.  I love the "Pumpkin" 2-seater lander can too much to give up on HGR just yet, but in case an update lands that breaks HGR completely (or I just get tired of making config repairs), here are a couple of other addons which add 1.875m parts:

* [**Socke's extension**](http://forum.kerbalspaceprogram.com/index.php?/topic/88780-wip-sockes-parts-1875m-extension/) only has fuel tanks and separators/decouplers, and Socke hasn't been around since last October either.  Thankfully, Merill has made [**an update**](http://forum.kerbalspaceprogram.com/index.php?/topic/88780-wip-sockes-parts-1875m-extension/&do=findComment&comment=1929389) for 1.0.x.
* Angel-125's [**Mark One Laboratory Extension**](http://forum.kerbalspaceprogram.com/index.php?/topic/94352-alpha-105-mark-one-laboratory-extensions-mole-v03/) is more complete and (more importantly) is actively developed and maintained.  It doesn't have a full range of engines, but there are enough adapters and multi-couplers to let stock engines fill in, and it has pretty much everything else, including a 1.875m "backseat" extension to the Mk1 command pod and a lab.

##Download and install

* [**GitHub**](https://github.com/Kerbas-ad-astra/HGR-Community-Fixes/releases)
* CurseForge

From there, just unzip the "HGR" and "HGRCommunityFixes" folders into your GameData directory.  (If you've already renamed internal2_RPM.txt to internal2_RPM.cfg, you'll be asked if you want to replace it -- the files are identical, so it doesn't matter which you choose.)

##Version history and changelog

* 2016 02 06 (1.0): Initial release.
* 2016 02 14 (1.1): Vegetable Gardening
	* Docking port, tech tree, and Windowshine patches added.
	* ASET IVAs for SoyJuice, Onion, and Leek pods.
* 2016 02 15 (1.1.1): Bugfixes
	* Removed ASET IVA files (they need more attention)
	* Added some cost updates to the LS patches (the cost of a part is its "wet cost", so when resources are added, the cost has to be increased as well).
* 2016 03 01 (1.2): Heat Treatment
	* Re-balanced the thermal properties of the engines.  They should now be no more prone to overheating than stock engines.
	* Fixed Radish and Spud heat shield patches to stop them from turning black when ablated.
	* Fixed lab patch (thanks speedwaystar!)
* 2016 04 27 (1.3): Naming Day
	* Fixed cost changes of life support patch to accommodate the updated price of USI-LS supplies.  Note that, because this change was made in a CRP update for 1.1, **this and subsequent versions of HGR Community Fixes are not compatible with KSP 1.0.4 or 1.0.5.**
	* Added a patch to delete RPM internal elements when RPM is not present, to reduce grumbling in the log.
	* Added a patch to rebalance the mass of the fairings and fix the Heavy LES tower.
	* Added support for BahamutoD's Animated Engines.  (It's a bit late, since BDAnimationModules needs updating for 1.1, but we're ready when it is!)
	* Added tags and part test constraints, and nicknamed the engines ("Grizzly", "Sunbear", and "Teddy")
	* Made SoyJuice solar panels non-retractable (and added a warning to their description).
* 2016 05 28 (1.3.1): Seared Tubers
	* Updated thermal values of crew pods.
	* Fixed a couple of tags.
* 2016 06 26 (1.4): Ogres are like Garlics
	* New G4-LK "Garlic" supply module to ease the overstuffing of the Lima.  Note that **the Lima no longer has life-support or KIS inventory storage** -- that's been moved into the Garlic capsule.
	* Added support for DeployableEngines (Nertea's plugin used for e.g. Cryogenic Engines).
	* Fixed some spelling in part descriptions.
	* Re-titled HGR's 1.875m fairing, to distinguish it from MOLE's.
* 2016 09 10 (1.4.1): Remote Control
	* Removed the RT patch (it's in RT now).  Therefore, **this and subsequent versions of HGR Community Fixes are not compatible with KSP 1.1.0-2.**
	* Added a texture-name-fixing patch.
	* License changed to GNU GPL v3 (or later).
* 2016 10 12 (1.5): Plus Ultra
	* Updated for KSP 1.2:
		* AntennaRange patch removed.  (Since AntennaRange is superseded by the stock CommNet.)
		* CommNet and KerbNet support added.
		* New RCS plume and sound effects added to RCS parts.
* 02016 10 29 (1.5.1): Transform and Deploy
	* Fixed transform references for solar panel/antenna.
	* Updated Edamame service module to ModuleEnginesFX.
	* Moved parts to new categories (Engine, FuelTank, Coupling, Thermal, Payload, Electrical)
	
##Roadmap

Nothing much -- just keeping things up-to-date.  Unless somebody else makes an up-to-date 1.875m 2-seater lander can and 2-seater blunt capsule -- that's about all I'd need to be done with HGR!

##Credits

Thanks to speedwaystar for the Windowshine patch, and for contributing to the tech tree and docking port patches, rasta013 for contributing to the lab patch, fatbrother for the fairing mass fix, pacbard for conributing to the engine patch, Sp4C3M0nk3Y for the ASET IVAs, and ZentroCatson for contributing to the KIS patch.

And of course, thanks are owed to OrionKermin for HGR itself!  We wouldn't have anything to fix if not for him.  :wink:

##License

HGR Community Fixes is copyright 2016 Kerbas_ad_astra.  Configuration files are released under the [**GPL v3 license**](https://www.gnu.org/licenses/gpl-3.0) (or any later version).  Any redistributions must use a different name and folder (per section 7c).  All other rights (e.g. the HGR Community Fixes logo) reserved.