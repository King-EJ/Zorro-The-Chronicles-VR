ZORRO THE CHRONICLES VR  v0.1.1 (test build) - Unity 2019.4.34f1, IL2CPP x64, built-in renderer
===============================================================================================

**TEST BROKEN RELEASE**

<img width="1024" height="1536" alt="Zorro_ The Chronicles in VR" src="https://github.com/user-attachments/assets/0ce4e641-06cf-467f-988d-938421af6ecf" />



Install
-------
unzip to game folder, only tested with virtual desktop XR

Start the game with -force-d3d11 (Steam: right-click the game > Properties > Launch Options)

**[Nefarius ViGEmBus](https://github.com/nefarius/ViGEmBus/releases) support - with the driver installed (ViGEmBusSetup_x64.msi in the zip) the VR
        controllers are a real virtual Xbox 360 controller ([Controls] InputMethod = Auto / ViGEm / InputSystem).**

The views
---------
TAP R3 (right stick click) ...... first person <-> third person. Hold R3 (0.5 s) = the game's own R3.
RIGHT STICK DOWN (third person) . the game's camera <-> following behind Zorro ([View] RightStickDownStyle).
THIRD PERSON (start) ............ the game's camera (the right stick's left / right moves it like on a pad, your
                                  view turns with it), or following behind Zorro ([View] Follow).
FIRST PERSON .................... you are at Zorro's head (head hidden); his arms follow your controllers.
Cut-scenes / animated cameras / the scope use the game's camera ([View] GameCameraInScenes).

Combat (first person)
---------------------
Swing the RIGHT controller ...... X        ([Weapons] SwingRightButton)
Swing the LEFT controller ....... Y        ([Weapons] SwingLeftButton)
[Weapons] SwingMelee (on), SwingSpeed (how fast a swing must be, m/s), SwingCooldown. The X / Y buttons work too.

Weapons in your hands (first person)
------------------------------------
The SWORD is in your RIGHT hand and the WHIP in your LEFT hand (off), pointing where the controllers point (only in your
view - the game's own weapon handling is unchanged). [Weapons] SwordInRightHand, WhipInLeftHand, ShowWhipAlways,
SwordOffset / SwordRotation, WhipOffset / WhipRotation.

Telescope
---------
While the telescope is up, the game's zoomed picture is in a round lens in front of your eyes (it turns with your
head). [Scope] ScopeLens, LensSize, LensDistance, LensResolution (also in the VR menu).

Live hand adjust (first person)
-------------------------------
HOLD BOTH GRIPS 1 s (or VR menu "Live hand adjust"). The game gets no input meanwhile:
  right stick up / down = tilt the hand, left / right = turn it      hold RIGHT TRIGGER + right stick = roll
  left stick = move the hand left / right / forward / back           hold LEFT TRIGGER + left stick up / down = height
  X = switch left / right hand     B = reset that hand     A (or both grips again) = done (saved)
The sword / whip in that hand moves with it.

Arms
----
First person: Zorro's hands follow your controllers (two-bone arm IK). Each hand can be moved / turned on its own
in the VR menu ("Hands" -> "Adjust hands ..." or the Left hand / Right hand rows): right / left, up / down,
forward / back, tilt, turn, roll. [Arms] HandsFollowControllers, InThirdPerson.

Controls (the VR controllers are an Xbox pad)
--------
  
  Right stick up ............... d-pad up ([Controls] RightStickUp)
  
  Right stick down ............. third person: game camera <-> follow
  
  Right stick left / right ..... turn (first person / follow); moves the game's camera (game camera view)
  
  A + B together ............... Start
  
  X + Y together ............... Back
  
  **Tap both stick clicks ........ re-centre the view**
  
  Hold both stick clicks 1.2 s . VR settings menu (right stick = choose / change, A = select, B = close)


CHANGES
-------
v0.1.5

  - Marked enemies: the game's marker on the HUD (in the wrong place in VR) is removed; a marker floats above
    each marked enemy in the world instead, seen through walls. (VR menu > Enemies; [Camera] MarksIn3D / MarkSize.)
  - Rock: while holding a rock to throw, point the LEFT controller where to throw - the aim turns there by itself
    (the right stick still works and takes over while you push it). [Controls] AimRockWithLeftHand.
  - Telescope: the lens sits on your RIGHT controller and follows it; point the hand where to look and the
    telescope turns there (no right stick needed; pushing it still works). [Scope] LensOnRightHand / AimWithRightHand.
  - First person: the hearts and the lightning float by the LEFT hand, the objective by the RIGHT hand.
    [HandHud] HudOnHands, HandHudScale, Left/RightPanelPosition.
  - The whip is no longer in the left hand (VR menu > Hands to turn it back on).
  - The sword has its own place on the controller: adjusting the hand no longer moves it. Live hand adjust:
    X now goes right hand -> left hand -> sword, so the sword can be adjusted on its own too.

Issues
-
* enemy disappear and some of the world
* throwing rock have to turn controller upside down to move aim
* player go transparent in1st person sometimes
* telescope take some getting use to,can move with right stick and with moving right hand

Disable: to disable Mod rename winhttp.dll to winhttp.dll.bak

[VR Mod Manager](https://github.com/King-EJ/VR-Mod-Manager/releases/tag/VRModManager)

LICENSES
-
Uses Astien's OpenXR bridge. Free, non-commercial.
