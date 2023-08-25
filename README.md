# <center><U>**Triple-Decky Filament Block**</U></center>

## Filament block with  triple decks for ERCF V1/V1.1, Sturdy Bunny and ERCF V2.

## What is it ?

**Triple Decky** is based on the Sturdy Bunny filament block from **Sneakytreesnake** that incorporate the MR85ZZ bearing making the need for bearing blocks obsolete. It is a replacement for the filament block on ERCF V1 and Sturdy Bunny. Its goal is to avoid the filament to move in or out the filament block while loading or unloading another gate.
To do that, the filament block consist in 2 hinged parts (decks), that are kept apart by magnets. The filament is lifted by 1 mm from the bottom BMG gear.
The tophat comes on top of the 2nd deck and has the top BMG gear as before.
An integrated tophat based on number 1 tophat locker to be used with Springy [from Moggieuk](https://github.com/moggieuk/ERCF-Springy/tree/main) on Rev B and C.
Although Rev B version still has the possibility to install the magnetic gate, it is normally not needed anymore.
It will not be possible to install the magnetic gates on Rev C.
The width is 23.05mm as the latest Sturdy Bunny filament block that incorporate the bearing in the block.
To take all the benefit of the Trple Decky Filament Block, it is recommended to use a good buffer system (preferably a single loop buffer) The PTFE tube should not apply down force on the ECAS so the magnet can do their work correctly.
For people who needs a bypass block, there will be one incorporated in the "filament block end" of ERCF V2. A stand alone Bypass block that can be placed anywhere on the 2020 extrusion is also available on the triple decky Github. (Bypass_with_ECAS.STL) 

## Summary.
* **[Bom](#bom)**
* **[Printing Tips](#printing-tips)**
* **[Cleaning tips](#cleaning-tips)**
* **[Assembling tips](#assembling-tips)**
* **[Revision C for 3 positions servo "3PS" (Strudy Bunny & ERCF V2)](#triple-decky-for-3-positions-servo-brake-release)**
  * **[Important note about Rev C 3 positions servo](#important-note-about-the-3ps-version)**
* **[Revision C for magnet release brake (Strudy Bunny & ERCF V2)](#triple-decky-for-magnet-brake-release)**
* **[Revision B (Strudy Bunny & ERCF V2)](#triple-decky-rev-b)**
* **[TD for ERCF 1.1](#for-ercf-v1)**


## Latest updates.
* #### Stand alone Bypass Block with ECAS. 
     
   <center><img src="Images/Bypass.JPG" width="250" alt="C6 bearing">You can find it in stl/sturdy bunny</center>
  
* #### New Filament Path Rev C6_3. Read more about it [here](#update-6_3). 

* #### Triple Decky Rev C for 3 positions servo STLs. Make sure to read the [Important Note Below](#important-note-about-the-3ps-version) first !!!

 * #### Triple Decky Rev. C. Read the details [here](#triple-decky-rev-c)

  
## **Yet in development :**
* **ERCF V2 :** at this moment, ERCF V2 is in development by a team of designers. Lots of things have been developed and are tested, but regarding the filament blocks, no decision have been taken on which version of Triple Decky or another type will be used.
  * Mods in progress :
    * Sturdy Bunny: https://github.com/sneakytreesnake/SturdyBunnyProject
    * Springy: https://github.com/moggieuk/ERCF-Springy/tree/main
    * Ejection Assisted Purge: https://github.com/bombela/EjectionAssistedPurge
    * Binky: https://github.com/mneuhaus/EnragedRabbitProject/tree/main/usermods/Binky
    
   



**I have re-structured this GitHub to show only the latest versions of each type. All previous STLs are available in the Archives folder.**

## BOM.
For each block you need :  
  * #### Rev B.
    * 1 M3x8 SHSC (to mount the base on the 2020 extrusion)
    * 1 M3x18 SHSC (to mount the latch on the base)
    * 2 6x3 magnets (between the base and the filament path)
    * 1 ECAS (on the filament path)
    * 1 set of BMG (on the D-shaft in the base and in the top hat)
  * #### Rev C magnet release trap.
    * 1 M3x8 SHSC (to mount the base on the 2020 extrusion)
    * 1 M3x18 SHSC (to mount the latch on the base)
    * 1 M3x3 set screw. Length: from 2 to 3mm (to install in the trap) (M3x2 can be found in BMG).
    * 3 6x3 magnets (between the base and the filament path and at the back of the filament path)
    * 1 ECAS (on the filament path)
    * 1 set of BMG (on the D-shaft in the base and in the top hat)
  * #### Rev C 3 positions servo release trap.
    * 1 M3x8 SHSC (to mount the base on the 2020 extrusion)
    * 1 M3x18 SHSC (to mount the latch on the base)
    * 1 M3x3 set screw. Length: from 2 to 3mm (to install in the trap) (M3x2 can be found in BMG).
    * 2 6x3 magnets (between the base and the filament path)
    * 1 ECAS (on the filament path)
    * 1 set of BMG (on the D-shaft in the base and in the top hat)
 
## **Printing tips:**
  * Make sure your printer is well tuned, especially the first layer height. If it is too thick, the brake (trap) will be too thick and will not move freely inside the filament path.
  * All STL were tested OK with ABS and ABS+ 
  * Use voron standard print profile ( I use Andew Ellis ABS print profile).
  * The 3 main parts are fitting together using a kind of hinge. They should fit together without filing and with a little bit of play. 
  * Make sure that the rectangular hole in the filament path Rev C is clean so the trap/brake can fit loosely in. There should be 0.5mm clearance.
  * For unknown reason, Super Slicer and Prusa slicer reports 6 open edges on the filament path STL. **DO NOT try to fix it**, otherwise you will have support that are filled up with infill and more than one perimeter thick. 
  * Make sure you have "Thin wall" enable, otherwise you won't have supports. Set also the speed for thin wall around 50% of the external perimeter speed.

## **Cleaning tips:**
  * All support should come off very easily.
  * There should be very little part cleaning necessary
    * Using a 2mm drill bit, clean the filament path
    * using a needle file, clean the rectangular hole where the trap is going in on the filament path
    * The trap part should have a thickness of 3.05mm, use a file to make it <= 3.05mm or tune your first layer.
    * On the screw trap part you need to make sure that there are no plastic between the thread of the set screw and the filament. Use a sharp x-acto knive to open the space between the 2 holes.
   
    <center><img src="Images/C-trap.JPG" width="250" alt="C6 bearing"></center>
    
    * On Rev C with magnet brake release, make sure the hole for the back magnet is clean, the magnet should go down against the bottom of the hole.  
    * On the tophat up to version C6.2 it could be possible that depending on the type of ABS(+) you're using, the tophat does not move as freely as needed. To solve that, you can cut or file down one layer off from the tang on the support side. This is fixed in the next version C6.3. I only encounter that problem with my ESUN Green ABS+.

    <center><img src="Images/C6-Tophat-62b.JPG" width="250" alt="C6 bearing"></center>


## **Assembling tips:**
  * Rev B is self explanatory. The 3 parts goes together by sliding the tangs into the correponding cavities that makes the hinges.
  * Rev C need a bit more attention to assemble the filament path on the base.
    * 1. Insert the M3x8 SHCS screw into the side hole of the base before installing the filament path. You will be able to access the screw through the filament pass later. (If you want to use 4 magnets, than you need to install the base on the 2020 extrusion before installing the magnets and filament path. 4 magnets are normally not necessary.)

      <center><img src="Images/C6-M3x8.JPG" width="250" alt="C6 bearing"></center

    * 2. Insert the magnet into the middle holes of the base and the filament path. The magnet must repell each other.
      * Optionally, you can use another set of magnet into the side holes if needed. In that case, the screw will be unaccessible without disassembling the parts
    * 3. Insert the trap into the female dovetail.
      * If you use the screw trap, insert the set screw at a slight angle. The 2 holes are angled by about 2°. Insert the set screw in the top hole. <BR>
      The set screw can be :
        * M3x3mm
        * M3x2.5mm
        * M3x2mm, the same that you can find in the BMG.   
       
      <center><img src="Images/C-trap-angle.JPG" width="250" alt="C6 bearing"></center>

    * 4. Align the filament path above the base so they are parrallel and the top of the brake (trap) is "almost" inside his corresponding hole in the filament path and the tang of the hinge is just above the cavity of the base. 
     
      <center><img src="Images/C6-snap.JPG" width="250" alt="C6 bearing"></center>
    
    * 5. Press firmly the filament path into the base. It snap into place easily.
    
      <center><img src="Images/C6-snap2.JPG" width="250" alt="C6 bearing"></center>

  * Magnets orientation.
  
       <center><img src="Images/Magnet.JPG" width="150" alt="C6 bearing"><img src="Images/C6-magnets.JPG" width="450" alt="Magnets"></center>

 ## Triple Decky for Sturdy Bunny build on a 2020 extrusion. 
 ### Triple Decky Rev C
   **It is an evolution of Rev B. with the following new features.**
   *  It has a kind of brake to press against the filament when the gate is not selected. The exit side of the filament path can lift up about 0.5 mm, enough to make the filament touching the brake part (trap). To release the brake it will use either :
        *  with a magnet that will be pushed back by the encoder magnet.
        *  by using a special tophat that will need a 3rd position of the servo to be able to move the selector. (software in development)<p>
   * The brake part will be easily replaceable in case it breaks.
   *  The multi-color tag plates will be the same for input and output side. (Same as in version B4 Base)<p>
   *  The use of the old magnetic gates will be **impossible** on that version.
   *  If you are using Happy Hare software, you should decrease the "parking_distance" in the ercf_parameters to about 15 so the filament parks inside the trap.
   *  It is normal that the filament does not pass the trap when inserted manually. When the gate will be selected, Happy Hare will load it without problem. If you want to lock it inside the trap, than you need to push down the exit side of the filament path with your finger and insert the filament about 5 mm further.<p>
  
### **Triple Decky Rev C6 magnet brake release or 3 positions servo.** 

#### Update 6_3 
 This update concern all **Filament Path revision B and C for Sturdy Bunny**. The ECAS is moved 4mm out to enable the insertion of the PTFE tube inside the part. I recommend to use it over the previous versions.
 * This allow for easy threading of the filament and keeps also the geometry for Endless Spool function.
 * It avoids the ECAS to go slowly out of its cavity after some time.

<center><img src="Images/C63.JPG" width="250" alt="C6 bearing"><img src="Images/Diff-C63.JPG" width="250" alt="C6 bearing"></center>


      
#### Update C6 
This is an update from Rev C5 that fixes the following issues:
  * wall around the bearing cracks
  * filament path output side rubbing on the encoder and get pushed down. 
  * **It has the following new feature :**
    * thicker wall around the bearing
    * output face of the filament path is tilted 4° to avoid rubbing on the encoder cart
    * new tophat to match the brake release magnet new position

        <center><img src="Images/C6-bearing.JPG" width="250" alt="C6 bearing"> <img src="Images/C6-backside.JPG" width="250" alt="C6 output face"></center>

  * **Warning:**
          * C6_x base need to have C6_x filament path
          * C6_x filament path need to have C6_x tophat
          * C5_x base is compatible with C6_x filament path
          * C5_x filament path is compatible with C6_x tophat
          * For all Rev C, only the integrated tophat are available, and needs the Springy servo holder to work. (see above in mods in progress) <p>
      <p>
           

### **Triple Decky for 3 positions servo brake release.**
  
   * This version uses the servo to push the filament path down so the filament is free to move when the gate is selected.
   * When the gate is not selected, the filament will be hold still by the trap.
   *  New integrated tophat based on number 1 tophat locker to be used with Springy [from Moggieuk](https://github.com/moggieuk/ERCF-Springy/tree/main) 
    
      <center><img src="Images/C6-3PS-in.JPG" width="250" alt="C5 in"> <img src="Images/C6-3PS-out.JPG" width="250" alt="C5 out"></center><p>
      <center><img src="Images/C6-3PS-cut.JPG" width="250" alt="C5 cutout"> <img src="Images/C6-3PS-trap.JPG" width="250" alt="C5 trap"></center>
  
#  **IMPORTANT NOTE ABOUT THE 3PS VERSION.**
   *  **If you want to test the C6 with 3 positions servo YOU HAVE TO have access to the latest Happy-Hare software (HHv2) that support the servo 3rd position. Otherwise IT WILL NOT WORK. It is in beta for a few people at this moment. If you are one of those beta tester, you can try this Triple Decky C6 3PS. <br>IF NOT, WAIT UNTIL IT IS FULLY RELEASED.<br> The actual KlipperScreen for Happy Hare needs also a special updated version.**
   * The base is the same for both Rev C versions (Triple_Decky_Base_C6_0.stl).
   * The taps are the same for both Rev C versions (Traps folder).
   * If you are already using the magnet version, you can still use it if you print the universal tophat ([a]Triple_Decky_Tophat-integrated_Universal_Mag&3PS_C6_0.stl). **DO NOT USE THIS STL IF YOU DO NOT HAVE ENABLED THE 3rd POSITIONS FOR SERVO IN YOUR SOFTWARE!!!**
   * If this is your first use of Rev C 3PS, then it is better to use the dedicated tophat for 3PS ([a]Triple_Decky_Tophat-integrated_3PS_C6_2.stl).
   * Optionally you may want to use the special servo arm with rounded edges (Servo Arm MG90S_for_3PS.stl or Servo_Arm_Savox_for_3PS.stl) .
   * **Software parameters** 
     * Add "servo_move_angle: (move position angle)" in mmu_parameters.cfg
       * **For MG90S**
           * servo_move_angle: 45
           * servo_up_angle: 24
           * servo_down_angle: 115
          <p>
       * **For Savox SH0255MG**
           * servo_move_angle: 95
           * servo_up_angle: 115
           * servo_down_angle: 45
         
      * Change the "encoder_parking_distance:" in mmu_parameters.cfg so the filament parks in the trap. (for me I change it to 15, it was 23) 
    * **Servo positions**
      * Servo Up. (trap released / print without sync)
         <center><img src="Images/Servo-up.JPG" width="250" alt="C5 in"></center>
      * Servo Move. (trap locked / selector movement)
         <center><img src="Images/Servo-move.JPG" width="250" alt="C5 in"></center>
      *  Servo Down. (trap released for Load/unload or print with sync mode)
         <center><img src="Images/Servo-down.JPG" width="250" alt="C5 in"></center>      <p>
 

### **Triple Decky for magnet brake release**

   * This version uses the encoder magnet to push the filament path down so the filament is free to move when the gate is selected.
   * When the gate is not selected, the filament will be hold still by the trap.
  *  New integrated tophat based on number 1 tophat locker to be used with Springy [from Moggieuk](https://github.com/moggieuk/ERCF-Springy/tree/main)
            

       <center><img src="Images/C5-in.JPG" width="250" alt="C5 in"> <img src="Images/C5-out.JPG" width="250" alt="C5 out"></center><p>
       <center><img src="Images/C5-cut.JPG" width="250" alt="C5 cutout"> <img src="Images/C5-trap.JPG" width="250" alt="C5 trap"></center>


### **Triple Decky Rev B**

   * The output side of the filament path has been tilted by 4° to avoid rubbing on the encoder when the selector is moving.
   * The input side tag plate is rotated 90° for better printing without support.
   * New multicolor tag plates for 12 carts on the input side.
   * New multicolor gate plates for 12 carts on the output side to replace the magnetic gate. 
   * New integrated tophat based on number 1 tophat locker to be used with Springy [from Moggieuk](https://github.com/moggieuk/ERCF-Springy/tree/main)  
   * optional base to use the old magnetic gates. In that case, the small part of the hinge of the filament path must be cut at the mark.
   * The latch has an optional set screw to apply a little bit of friction on the filament. This help the filament to stay still in case of vibrations.<p>
   * Since this version has no real brake system. It is better to use a single loop buffer system that provide more stability of the filament when it is in the buffer.
  
      <center><img src="Images/B4-in.JPG" width="250" alt="Triple Decky for Sturdy Bunny"> <img src="Images/B4-out.JPG" width="250" alt="Triple Decky for Sturdy Bunny"> <img src="Images/B4-side.JPG" width="250" alt="Triple Decky for Sturdy Bunny"></center>
           
 
## **Triple Decky for ERCF V1**

   * This is for the original design that is build with M5 all threaded rod. This version will not be developed further because almost all users / builders are moving to Sturdy Bunny, or the coming (soon) ERCF V2.<p>
   
      <center><img src="Images/TD%20for%20ERCF-V1.JPG" width="250" alt="Triple Decky for ERCF V1"></center>

  
