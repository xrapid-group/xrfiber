
<script type="text/javascript" async
  src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.2/MathJax.js?config=TeX-MML-AM_CHTML">
</script>


xRFiber Standard Operating Procedure
---

Document Revision: 1.1

App Version: 1.60 Build: 597

# 1. PURPOSE

This document describes the standard operating procedure of the xRfiber platform.

xRfiber comprises a motorized microscope that is wirelessly operated by an iPhone or iPad, and a software to drive the microscope. It is dedicated to the measurement of fibers in air samples, following a large number of standards or recommendations in accordance with local rules. The microscope is operated in phase contrast, the images are captured by the iPhone or iPad and analyzed locally by an embedded artificial intelligence.

Although a training is provided when a unit is deployed in a laboratory, this document should also be read, understood and referred to when questions arise.

If an information is requested, particularly if relevant and not found in the document, the user is welcome to contact [support@xrapid-group.com] for any further question.

# 2. CONTEXT

-   These instructions are for the use of researchers, technicians and operators in general who are performing air samples fiber diagnostics.
-   This SOP contains general guidelines for the analysis of samples only. Please refer to relevant standards for samples preparation.
-   This SOP is not a substitute for the standards, the machine and software are used within the frame of standards and/or recommendations but do not replace them.

## 2.1. Main characteristics

xRapid Group has developed a fully automated microscope, patent pending, which consists in a phase contrast microscope (PCM) retrofitted with a set of motors to control the stage movement in three orthogonal directions (x, y and z) with various accuracies. This enables a full sample (a quarter disk of 1” diameter mounted on a glass slide) to be imaged within a few minutes. A series of images are taken by an iPhone or iPad at increasing depths, from which an autofocus measure is calculated to image the next field. At the same time, a convolutional neural network (CNN) is used for our AI to characterize the objects in the field of view. All the analysis is performed locally on the device, none of the images are uploaded to a server, so that remote work in a poorly connected area is permitted. While we usually refer to AI as Deep Learning, one should notice that xRfiber system is not self-learning: all the data has been extracted by humans, and validated by humans. The system shipped is not evolving between updates of the app, which enables to guarantee its performance and pass a certification.

## 2.2. Equipment specifications

### 2.2.1. General

-   Phase contrast microscope, with phase condenser ring 40×.
-   Objectives: 40× PCM (5 spots on the turret, 10× PCM optional)

### 2.2.2. Illumination

-   Kohler illumination
-   LED light source, 3W

### 2.2.3. Power

-   12V-3A power source for 100-240V 0.8A mains, EU-UK-USA-AUS adapters (CE)
-   USB-A plug charge only for iPhone/iPad Pro 10.5’’ (5V, 2A), USB-C plug charge for iPad Pro 11’’ (5V, 3A and 9V, 2A)

### 2.2.4. Eyepiece

-   Two eyepieces, standard 30mm tube diameter.
-   One third eye with a 10× (23mm diameter) eyepiece mounted on collapsible tube, factory centered, on which a cradle support for iPhone/iPad is attached.

### 2.2.5. Motorized stage

-   X&Y displacement by steps of 125µm and 220µm, respectively
-   Z displacement by steps of 0.5µm or 0.25µm in sequences
-   X course: 75mm
-   Y course: 30mm
-   X&Y error: ±5µm over 18mm (forward and backward displacement of 40 steps)
-   Speed: 15ms/step (X&Y), 9ms/step (Z)
-   Control of coarse and fine displacement by software
-   Stage piloted via Bluetooth or Ethernet through the control app

### 2.2.6. Control machine

-   iPhone 7 or 8
-   iPad Pro 10.5”, iPad Pro 11”
-   Additional devices possible, requires additional mounts
-   Power adapter (Apple standard, fitted to region of purchase)
-   Must be connected to the internet at least once a month for authorization

### 2.2.7. Control app

-   Fully automated diagnostic with return to the original point of measure
-   Average diagnostic time per slide lower than 3 minutes
-   Reproducibility better than 2%
-   Test log (journaling) and QC checks
-   Exports results to PDF and Excel spreadsheets (single or grouped)
-   Accuracy tested vs. IHPAT samples from rounds of last 4 years, all passed
-   Confidence interval 95% Poisson distribution implemented
-   Artificial intelligence based on convolutional neural networks trained by expert (machine learning), validated on 30’000 fields. This model is fixed in time, it requires a software update to evolve
-   Standards supported: NIOSH 7400 (Type A & B), OSHA id 160, NOSHC-3003, IRSST 243-1, HSG248, NF X43-269.

### 2.2.8. Operation details

-   Working capture resolution at 40× is ≈14 pixels per µm
-   Scale and gratings/grids displayed by software, factory calibrated to standard traceable micrometer calibration slides (Ted Pella slides 2280-11, 2280-13, 2280-15)
-   Virtual Walton-Beckett graticule displayed in app. Dimensions within 0.5% tolerance on 100µm WB graticule diameter
-   Objective and optics train in conformity with the HSE/NPL Mark 2 calibration slide.

### 2.2.9. Accessories

-   Telescope for ring position adjustment
-   Leveling tool
-   Dust protection bag and silicon dust cap, lens cleaning paper
-   Set of Allen/Torx wrench
-   Template for slide preparation

### 2.2.10. Controller (optional)

-   Nimbus bluetooth controller
-   Controller paired permanently to the iPhone/iPad
-   Two joysticks (left/right) for coarse/fine displacement, respectively
-   One D-Pad (left) for coarse focus adjustment
-   4 buttons, right, for fine focus adjustment

## 2.3. Standards and paths

xRfiber supports a large number of standards, which come with specificities, whether they are about the objects counted (for example, some standards specifically request *not* to count objects that are touching debris, while others have different strategies), or about the path that one must apply to scan the sample.

The following standards are currently supported:

-   NIOSH 7400 (Type A & B)
-   OSHA id 160
-   NOSHC-3003
-   IRSST 243-1
-   HSG248
-   NF X43-269
-   NBN T 96-102

Four sample geometries and therefore paths are supported: quarter disk oriented right or up, and half disk oriented horizontally or vertically.

# 3. SAFETY NOTES

-   Always carry the microscope with two hands, wear protective clothing and shoes when moving equipment. It is advisable to place one hand under the base of the box for extra support.
-   When opening the box, make sure that the top is facing upwards.
-   If the microscope is stored in a box, always ensure the door is locked before picking up the box.
-   Never disassemble the microscope on your own without xRapid-Group instructions and guidance as doing so may damage it and null the warranty.
-   Turn off and unplug from the power supply before moving the microscope.
-   Secure the turret of the microscope before and when moving the microscope.
-   Never use coarse focus on your microscope — this known is locked. Only the fine focus is available. The coarse focus knob is blocked, and using it will damage the z-movement of the microscope.
-   Make sure your workstation is set up ergonomically to use the microscope.
-   Make sure the microscope is not stored in direct sunlight, nor stored in rooms where large temperature variations are expected. Normal temperature usage is within 15 to 25 degrees Celsius.
-   Make sure the microscope is regularly electrically tested and tagged. Only use the provided electric cable and adapter. Choose a stable power source.
-   Wear protective clothing, gloves and goggles preferably when preparing the slides, and operating the microscope.
-   Never touch the lenses of the microscope with naked fingers: objectives, eyepieces and eyepiece on the trinocular.
-   Only use special lens paper to clean the optics.
-   Never touch an electric outlet with wet hands.
-   Do not open the back of the microscope without being grounded, as this may result in electric shocks/hazards.

# 4. PREREQUISITES

The following items are required for the operation of xRfiber platform.

-   A cleared and clean laboratory space, if possible with constant lighting and in a low vibration environment
-   A free power outlet
-   At least one dedicated technician
-   An internet connection, active during the installation and at least once a month on the first day of the month
-   An Apple mobile device: iPhone 7, iPhone 8, iPad Pro 10.5” (2018) or iPad Pro 11” (2019) are all compatible with the hardware
-   An iCloud account and AppleID (free iCloud account is good enough)
-   Depending on the standard, calibration slides
-   Depending on the standard of the laboratory, some QC slides
-   Optionally a networked printer.

# 5. RESPONSIBILITIES

It is the responsibility of the user to ensure that:

-   The microscope unit is functioning properly, and report to [support@xrapid-group.com][1] in case there is any doubt that it does
-   The power supply is connected to a stable source of 110V or 220V, depending on the local environment
-   The microscope unit it set in a proper environment, that the optics are covered and dust protected when the unit is not in use (see section 6.1)
-   The phase ring position is checked at least twice a day and/or before any other member of staff starts using the unit (see section 6.3)
-   A field blank is used regularly to check that the count is adequate, i.e. below 5.5 or 7 fibers/mm2 depending on the standard
-   An adequate number of slides are checked for quality control of the software (see section 6.5)
-   The user name on the main screen of the software, when operating the unit, is correct, for traceability purposes (see section 6.4)
-   The appropriate standard is selected (see section 6.4)
-   A copy of the standard in use locally is located close to the equipment for reference.

Additionally, the best results are obtained when:

-   The slides are well prepared: see separate SOP.
-   The initial focus is on the surface of the filter.

# 6. PROCEDURE

## 6.1. Hardware

### 6.1.1. Components

The xRfiber microscope components are shown in Figure 6.1, additional components in the box are shown in Figure 6.2.

1. Power Switch
2. Power Adapter Port
3. USB Charging Port
4. Fine Focus Adjustment Knob
5. LED Light Source with Field Iris Diaphragm
6. Condenser
7. Condenser Adjustment Knob
8. Phase Ring Holder
9. Condenser Iris Diaphragm
10. Microscope Stage
11. Stage Clip
12. X-Axis End Stops with Cover
13. 40x Plan PH2 Objective
14. Objective Turret
15. Oculars
16. Condenser Alignment Screws
17. Cradle Support Arm
18. Adjustable C-Mount Adapter
19. iPhone/iPad Cradle
20. Ocular Locking Screws

![][image-1]
Figure 6.1. xRfiber Microscope components


Figure 6.2. Additional components in the box

---- 
21. Protection Bag
22. Lens Cleaning Tissue
23. Slide Preparation
24. Level
25. Plug Adapter
26. Power Supply
27. Telescopic Eyepiece
28. Eyepiece Cap
29. Eyepiece Screws
30. Eyepiece WF10X
31. Allen Wrench (Alignment)
32. Allen Wrench H2.5
33. Allen Wrench H1.5
34. Torx T10  


### 6.1.2. Installation

1.  OPENING THE BOX

Upon opening your xRfiber unit, please use the checklist provided to confirm all items have been received: the checklist is on the top of the box when opening it. If something is missing, please contact support@xrapid-group.com.

![][4]

Figure 6.3. box contents

2.  GETTING THE MICROSCOPE OUT OF THE BOX

When deciding where to place the xRfiber Platform, consider the following:

-   The platform should be placed on a stable, level surface

<!-- -->

-   The platform should be placed conveniently as to minimize the need to move after initial setup

-   The area/room the platform is placed in should have consistent, even lighting as to prevent errors due to fluctuations in ambient lighting

-   Once a location has been selected, take the microscope out of the box and place it in the selected area

-   Remove the plastic wrapping from the microscope.

Verify that the head of the microscope (A) is aligned with the body (B). If not, slide head into alignment with the body by hand: apply a slight rotation of the head to align its edges with those of the body.

![][5]![][6]

Figure 6.4. Alignment of the microscope head

Verify that the adjustable C-Mount Adapter (n°18) is aligned with the head of the microscope. If not, use a Allen wrench H3 (not included) and adjust the adapter after loosening the screw.

Remove both Ocular Covers (n°35). Eventually use a air duster (not included) in the ocular openings to ensure that they are free of debris and dust.

![][7]![][8]

Figure 6.5. Installation of the eyepieces

3.  INSTALLING THE OCULAR (N°15)

If the ocular is not clean, use an air duster (not included), and/or the Lens Cleaning Paper (n°22) to clean it before insertion (no circular motion — always have a linear motion so that the dirt stays on the edges of the lens and does not spread over the lens).

If you cannot insert it, loosen the ocular locking screw(s) (n°20) with the Allen Wrench H1.5 (n°33) and try again.

4.  SECURING THE OCULAR (N°15)

Slowly tighten the screw with the Allen Wrench H1.5 (n°33) to secure the eyepiece.

5.  INSERTING THE TELESCOPIC EYEPIECE (N°28) FOR PHASE RING ALIGNMENT

If you cannot insert it, loosen the eyepiece locking screw (n°20) with the Allen Wrench H1.5 (n°33) and try again.

Insert the Telescopic Eyepiece (n°27).

Slowly tighten the screw with the Allen Wrench H1.5 (n°33) to secure the Telescopic Eyepiece (n°27).

6.  INSTALLING THE OBJECTIVE (N°13)

Rotate the turret so the available opening is askew from the optic train.

Carefully align and slowly tighten the 40X Plan PH2 Objective (n°13) in the available turret orifice.

**WARNING**: The objective is very fragile, please take care when handling

Turn the turret to align the objective (n°13) with optic train.

**WARNING**: Take care that the stage (n°10) is low enough in order to avoid collision with the 40X objective (n°13). If it is not the case, get the stage down using the Fine Focus Adjustment Knob (n°4).

7.  INITIAL CALIBRATION

#### Centering the condenser

-   With no sample on the stage, slowly close the field iris by turning the dial around it clockwise.

<!-- -->

-   As the edges of the iris come into the field of view, adjust the center of the condenser using the Condenser Alignment Screws (n°16) located on the front left and front right sides of the condenser.

-   When complete, the hexagon of the field iris should appear in the center of your field of view.

-   Begin turning the dial on the field iris counter- clockwise until the edges of hexagon are just outside the field of view.

#### Aligning the phase rings

**NOTE**: The phase rings should be aligned upon receipt of the unit, do not adjust the screws on the ring holder in the condenser unless you have formally verified misalignment.

Phase rings are aligned following this process:

-   With the telescopic eyepiece in one eyepiece, loosen the thumbscrew on the telescopic ocular and begin slowly pulling the telescope outward.

<!-- -->

-   Once you can see the light and dark rings clearly, tighten the thumbscrew to hold the position of the telescope. (DO NOT OVER-TIGHTEN)

-   If the light ring does not appear to sit neatly inside the dark ring, note the position of the two rings.

-   Remove the phase ring holder from the condenser.

-   Carefully adjust the position of the phase ring using the small hex key (Allen Wrench n°33) provided on the screws located on the back right and front right edges of the ring holder using 1/4-3/4 turns for each adjustment.

-   Return the holder to its place inside the condenser. Be sure that the notch for locking into the condenser is facing away from you and the handle of the ring holder is located on the right side of the condenser.

-   Check the position of the rings through the Telescopic Eyepiece, if they are still out of alignment repeat the previous three (3) steps and check again until they are aligned.

-   Once finished, return the telescopic ocular to its initial position and replace it with the standard Ocular (n°15).

![][9]![][10]![][11]

Figure 6.6. Illustration of the alignment of the rings (left and middle: misaligned, right: aligned)

6.  INSTALLING THE CRADLE (N°19)

Use the T10 screwdriver (n°34) to remove the 3 screws (n°29) from the eyepiece tube of the cradle.

Insert the Eyepiece WF10X (n°30) into the Cradle (n°19).

-   If the eyepiece is not clean, use an air duster (not included), and the Lens Cleaning Tissue (n°22) to clean it before insertion (no circular motion).

Replace the screws you had previously removed, making sure they do not run into the sides of the eyepiece.

-   Insert the screw approx. 1mm past the inner wall so that they keep the eyepiece in place but can also still be adjusted after attaching to the adapter.

Remove the two screws (n°37) located on the top of the back of the microscope.

Remove the C-Mount Adapter Cap and align the Cradle with the tube of the adapter sliding them together. (Note: the screw holes on the bottom of the Cradle Support Arm should line up with the holes you just opened in the previous step)

Attach the Cradle to the microscope using the two screws (n°36) you removed.

![][12]![][13]![][14]![][15]

Figure 6.7. Installation of the iPhone cradle

7.  ALIGNING THE CRADLE (N°19)

-   Unlock your device (iPhone/iPad) and open the “Measure” application (this comes installed on all iOS devices normally, if it is not installed search for it in the Apple App Store)

<!-- -->

-   Place the device across the stage of the microscope, taking care that it lays flat on the stage

-   If the stage is not perfectly level, you can try moving the microscope or rotating it on the table to find the most level position in the selected area

-   If you cannot get a zero (0) value after adjustments, take note of the level of the stage (degree and direction)

-   Remove the device and place it in the cradle

-   Loosen the locking knob on the adjustable C-mount adapter

-   Slide the C-Mount Adapter up into the eyepiece tube of the cradle

-   Make sure the adapter tube is fully inserted into the eyepiece tube completely past the screws in the eyepiece tube

-   While holding the tube and cradle together, adjust the height of the adapter until you get an optimal level in that y-axis direction

-   Tighten the locking knob on the adapter securely

-   Once the adapter is locked, start tightening the screws on the cradle tube to secure it to the adapter

-   Once secure, small adjustments can be made to the alignment through tightening/loosening these screws

-   If your stage was not perfectly level, adjust the cradle positioning so that the cradle orientation best matches the direction and twist/yoke angles of the stage level measured in the first place.

The ideal situation is shown below: the device both on stage and in cradle should show the same orientation, leveled at zero degrees in all directions.

![][16]

Figure 6.8. unbalanced (left) and perfectly flat orientations of the iPhone in its cradle and on stage

## 6.2. Device (iPhone/iPad) setup

After going through Apple’s initialization guide, ensure the following:

-   The device is logged into an iCloud account (this is required for location services to be active which is required for device use records).

<!-- -->

-   The device is connected to the internet (this is required to upload usage records for billing purposes).

Open the Apple App Store and select the Search tab in the bottom right of the screen. Search for “xRfiber” and the application should appear in the results list. Press the Install option and confirm the installation with your password/thumbprint. Once the application is installed, turn on the microscope and then open the application once the LED light source has finished blinking three times (approx. 3-5 seconds from powering on).

**NOTE**: when the microscope is switched on, the light first blinks three times. It is an indicator that the Bluetooth has been initialized and the microscope is now ready to interact with the Software (the xRfiber app).

## 6.3. Operating the software

The xRfiber app has many features to facilitate not only the diagnostic, but also the review of results. We will now examine the various screens and functionalities of the app.

### 6.3.1. Main screen

#### 6.3.1.1. Establishing a connection

When starting the app, the central button START MEASURE (5) is grayed out. After a few seconds, the app completes the connection to the microscope and is now ready to measure:

-   the Bluetooth logo (1) is circled

<!-- -->

-   the large hexagonal START MEASURE (5) button turns white and animates to a pulsation.

Notice that the Bluetooth logo (1) is more than just an icon: it is also a button that can be tapped again should the Bluetooth connection drop. It generally takes about 2-3 seconds to establish this connection.

**NOTE**: the Bluetooth standard comes with a few drawbacks. One of those is the failure to resume a connection when a service has been lost for a duration of 30 seconds.

Once a device is connected, the button (1) being circled, tapping the Bluetooth button again will show a pop up with the name of the device selected. In laboratory settings where more than one microscope can be connected via Bluetooth, this is used to change the iPhone/iPad assignment to another microscope.

**NOTE**: the Bluetooth functionality lets us discover the device based on the strength of the signal. If two devices are more than one meter apart, the iPhone/iPad will find the correct microscope, i.e. the microscope it is sitting on. If devices are closer, some mixing or confusion of signals may occur, and the device will have to be checked and connected manually using the pop up menu.

![][17]

Figure 6.9. Main screen in the disconnected state (left) and Bluetooth connected state (right)

#### 6.3.1.2. Elements

##### Operator

It is good practice, and **requested by most standards**, to have the operator (3) identified during testing. xRfiber offers the capability to have more than one operator registered on a device. When multiple operators are registered, the right and left arrows (2) are visible and circled, indicating that they can be tapped to select the next or previous operator in the list. When only a single operator is listed, the arrows do not appear. Alternatively, one can swipe left and right on the name of the operator and this will present the previous/next operator in the list.

Entering or changing an operator is done through the Settings option of the app.

##### Settings button

The Settings button (4) is always active, it leads to the parameters and options of the app. Will be used to set the standard, the operator(s) and optionally a printer.

##### Statistics line

The number of tests run this month (6) and today (7) are displayed on this line. These numbers are dynamic, they reset at the end of the day and the beginning of the month.

The last three tests are displayed in boxes (9) under the statistics, and can be used to navigate quickly to the detailed results of the test.

#### *Tests log*

The Tests Log button (8) props up the log of all the tests ever carried out on the device. Because the microscope does not keep in memory the record of the tests performed, but rather just the global count, the tests log may be different if two devices are used to drive the same microscope.

##### Light button

The light button (10) is used to switch on/off the microscope light source. When the microscope is connected the state of the microscope is highlighted under the button.

### 6.3.2. Settings screen

#### 6.3.2.1. Overview

The settings/options have 3 main categories, reached by tapping on the segmented control: User (1), Diagnostic (2), Print (3).

![][18]

Figure 6.10. Settings screens with the User (left), Diagnostic (middle) and Print (right) settings.

Notice at the bottom (4) the version and Build number between parentheses — communicate those when requesting support.

All changes need to be validated, by hitting the Save button at the bottom right of the screen. Cancelling restores the last saved options.

#### 6.3.2.2. User

All the users informations are private, and not exchanged with xRapid-Group: they are mainly used for app-generated reports, and QC/QA purposes. The printed, PDF or CSV reports will have all the information the user has entered in this section.

**NOTE**: For QC purposes it is impossible to change the name of the operator of a test once the test has started.

One must have at least one operator per device. Fill in contact details accordingly, and hit the Save button at the bottom right.

Tap the button (5) Add New Practitioner to have multiple operators on a single device: it will clear out the name field, and you will be free to Save this additional operator. There is no limit to the number of operators that one device can hold. On the other hand, there is a limit on the number of addresses (only one) an institution can have.

One can switch the user from the Main screen, or using the small arrows on the left and right of the name.

**NOTE**: it is good practice to change the operator of the software whenever the physical operator of the xRfiber microscope changes. At the same time, all the QC checks should be passed before a new run of slides is carried out.

#### 6.3.2.3. Diagnostic

8 Standards or Recommendations are currently supported:

-   NIOSH 7400 Type A & B

<!-- -->

-   OSHA id 160

-   NOSHC-3003

-   IRSST 243-1

-   HSG248

-   NF X43-269

-   NBN T 96-102

-   Custom: enter your own path

The main difference between them is mostly that some standards use a pseudo-random path (continuous measurements), and the sample geometry may also vary based on the regional recommendations.

All standards have been checked and tested against proficiency and live samples. xRfiber handles locale settings and filters peculiarities in the background. When there are more than one usual way to mount a sample as per standard, xRfiber gives a choice.

Three entries are possible to customize the tests:

-   The field blank value: following the user’s SOP, one may use a field blank correction. This correction is a number of fibers that need to be subtracted from the total number of fibers per 100 fields, and follows the recommendation NIOSH 7400. It will be subsequently applied to all new tests;

-   The capture scale, in pixels per micrometer: this value is calibrated using a traceable micrometer slide before shipping to the customer, and checked during first deployment and any servicing of the machine. Normal value is 14.1 with a maximum error of 0.5%. It is recommended that this value is checked once a month.

-   Number of Walton-Beckett graticules: the newest iPad Pro 11’’ are capable of large computations, and as such it does make sense to measure more than one field per image captured. The image resolution is not changing between the two modes, and we can benefit from adding a second graticule, i.e. using the image captured for two fields instead of one. When doing so, we perform half the movements and therefore gain all these displacement times. In the case where two graticules are used, one should check that the scale is the same for both, or refrain from using two if this is the case. Should both graticules not have the same scale, the user should contact [support@xrapid-group.com] for immediate intervention/remediation.

Notice that those last three settings are entirely optional.

The custom path is commented and color coded. It can be quite tricky to generate your first custom paths, we recommend that the support is contacted and the file is submitted before running it — there isn’t a check for consistency at the moment.

#### 6.3.2.4. Print

The easiest way to generate reports is to print them directly from the app. xRfiber has the capability to print to any wireless networked printer in a variety of formats. Tapping the printer or Add printer button will take you to the iOS print menu — this is a system feature.

xRfiber can print reports in color or monochrome, on A4 and US Letter paper. Should your printer handle double-sided prints, xRfiber will comply.

While most users want to export their results to a CSV (Comma Separated Values) file compatible with Excel or Numbers, it is useful for quality purposes to keep a daily log of the machine, and print it out at the end of the day. xRfiber facilitates this operation by letting the user select all the records of the day in the Tests Log to export or print them out.

### 6.3.3. Measurement screen

Once the device is properly setup, one can proceed to performing diagnostics. The Measurement screen is obtained when the hexagonal Start Measurement button is tapped on the Main screen.

When entering the Measurement screen, the microscope light source will turn on automatically. If it does not, the microscope is not properly connected to the iPhone/iPad via Bluetooth, and the connection should be re-established. Notice that failure to establish connection with the microscope stops the user from entering in the Measurement screen.

A default identifier (1) is automatically generated. It is grayed-out, and can be changed. Tapping this identifier will show the iOS keyboard (2), tapping the small X icon at the right of the field will dismiss all changes and the keyboard. Any identifier longer than one character can be entered. The case presented in Figure 6.11. enables the use of sequences: any string followed by a dash - and a number will be automatically followed by the the same string with the number incremented by one when the next test is launched. This is particularly useful when a file contains several samples with a resulting large number of slides.

![][19]Figure 6.11. Starting a diagnostic with changing the default test identification

![][20] The usual sequence is shown Figure 6.12: tap the Start Diagnostic hexagonal button (1), after which the diagnostic sequence executes automatically. One can adjust the position of the slide by tapping the Controls icon (2), which will bring up the in-plane control (3) and focus control (4). One can return to the start button by hitting the cross (5).

Figure 6.12. Illustration of entering a Diagnostic screen (right), start position being set up (middle), and diagnostic running (right)

As specified by standards, the diagnostic will stop when either the number of fields (6) or the number of fibers (7) reaches 100. The analysis can be stopped at any time by means of the Stop button (8). When the slide is heavily loaded with debris, as per standard recommendations the analysis does not complete (depending upon standards when 16 or 25% of the field is occulted, it should not be counted… xRfiber considers that the slide should be labeled as not measurable if 25 such fields are found). In this case, the user may want to force an analysis, which can be done using the switch (9). The Results will be explained in their own section hereafter.

Notice that the next time the analysis is launched, the test identification will now default to the next increment, if a dash was present in the first test diagnostic. It is possible to start a sequence at any number following the dash: this can be useful when a job is split in more than one series.

### 6.3.4. Results screen

![][21]The results screen has a large number of potential actions, beyond displaying the results of a test (last or past). The unified results screen is the same whether one accesses it following the completion of a diagnostic or going back to it from a Test Log.

Figure 6.13. Results screen

![][22]From this screen, one can access a record of the images captured by tapping button (1), or the export options with button (2). The date and time of the test are displayed in (4) and the test identification in (3). Notice that at this point, it is impossible to change the test identification. When the results screen is accessed, it always opens on the raw numbers resulting from the measurement: the total number of fibers and fields, for instance. As such, the segmented control (5) will always be selected by default. To change this display, one can tap the segmented control in (6) for example, to obtain the values in fibers per mm2. The Fields Counts (7) present the position and numbers of each and every field measured. The large button (8) leads back to the Tests Log screen or the Main screen depending where the unified result was displayed from.

Figure 6.14. Results screen (2)

The cognoscenti will have recognized that no volume is indicated on this set of results. Before calculating the density of fibers per volume, this is not required by xRfiber. When the fibers/cc segmented control is tapped, however, if the volume was never entered a box will pop up asking for the volume to be filled. This volume is entered in liters, it defaults to 1200 liters.

Important notes:

-   the volume cannot be changed after it has been set, obviously

<!-- -->

-   once the fibers/cc segmented control is tapped one **must** enter a volume.

When the volume has been entered, the fiber density will be displayed.

Notice that in all displays of the results, the quantity of fibers as well as the minimum and maximum bounds defined by the associated standard are displayed.

![][23]Figure 6.15. Statistics reports

![][24]As noted above, the fields counts are accessed from the Results screen. They indicate the number of debris and fibers measured in all the fields, together with their location. The plots on top can be swiped to display plots of the fiber distribution, the debris distribution. The fibers length vs. width is interesting as it gives an idea of the type of fibers one has measured. Both fiber and debris distributions are used to evaluate whether they follow a Poisson distribution (within 95% confidence), which is a measure of the randomness of the sample (and the base hypothesis of all standards).

Figure 6.16. Reviewing and exporting images

Depending upon options and version, the images of every field captured may be available from the Results screen. Navigation is quite standard for iOS, let us mention at least that one can pick and export images through that screen. Because of memory restrictions, one cannot select more than 50 pictures for export at a time. When an image is tapped, it is magnified. A double-tap on the magnified image will zoom in and out, pinch to zoom is enabled, and swiping to the right/left presents the next/previous image respectively.

Exporting results is performed through the Action button. It opens a set of options, to share as an image (in PNG format), as a printable sheet (in PDF format), to print directly using the iOS print server, or to save as comma-separated-value (two options). The latter is used to export to Excel or Numbers or other spreadsheet software. xRfiber normally manages the export format according to locale settings (i.e. a distinction is made between decimal separator and column separator depending upon the localization of the device). Should your export results come out poorly, do not hesitate to contact support@xrapid-group.com.

![][25]

Figure 6.17. Results export options

There are two options to export as CSV: one can either export the full result, or export the raw fiber counts data. In the latter case, a table of groups of 5 rows with 5 columns will be exported. All those raw counts are usually easy to copy and paste into LIMS systems.

The iOS system is complete, and as such it is possible to export to other networked devices. In cases of mixed ecosystems, eg. PCs which are frequently used in laboratory settings, one can export from the iPad or iPhone (running iOS 13) to a thumb drive and use this device to transfer data. Feel free to contact [support@xrapid-group.com] should you need a recommendation for adapters and/or thumb drives.

6.4. Calibration
---- 

The xRfiber microscope comes fully calibrated. Regular operation according to most standards require the use of two calibration slides for the resolution and the scale. The calibration is checked by xRapid during any visit and/or servicing. The user cannot check the calibration of the unit.

NOTE: the unit is calibrated for a specific set of optics provided, any change of the optics train requires a new calibration check. It is recommended not to change any of the optics, or send a request to support@xrapid-group.com before doing so.

### 6.4.1. Resolution

#### Basics

To test the resolution of the microscope, a HSE-NPL reference slide is used. The dimensions of the lines of each band are as follows, with Band Numbers | Line Width (um) |Maximum theoretical phase change for light (lambda=530nm) passing through a test line:

• 1 | 1.08 | 6.6°

• 2 | 0.77 | 4.7°

• 3 | 0.64 | 3.9°

• 4 | 0.53 | 3.2°

• 5 | 0.44 | 2.7°

• 6 | 0.36 | 2.2°

• 7| 0.25 | 1.5°

Each of the HSE standard test slides is an epoxy replica of the NPL Master. An impression of the lines is produced in a resin of refractive index 1.58 and is mounted on a standard glass microscope slide (76 x 25 x 1.2mm). This impression is sealed in another resin of refractive index 1.485 and covered with a standard (0.17mm thick) glass coverslip. To maintain a steady level of quality between slides HSL assesses each one. Only the test zone bound by the four sets of intense lines is examined assess the contrast of the band 4, 5, 6 & 7 and inspected for dust deposits that may cause light or dark spots. The whole slide is inspected for cracks, splits and other defaults in manufacture. Although these defects cannot be eliminated, all slides are considered to be satisfactory.

HSL certifies the test slides as satisfactory for use to set up phase contrast microscope and categorizes them into three sets:

1.  those that have band 4 fully visible and band 5 partially visible (red documents)

2.  those that have band 5 fully visible and band 6 partially visible (green documents)

3.  those that have band 6 fully visible and band 7 partially visible (yellow documents).

Each xRfiber microscope is tested with a band 5 slide (option 2, green document).

#### Results

![][26]

Figure 6.19. HSE-NPL slide bands as measured by the xRfiber unit

#### Method

The microscope is fitted with the same optics that are used for the automated diagnostic, i.e. an Olympus Plan CN ✕40 objective, the eyepiece, and an iOS device (iPhone 7/8, iPad Pro 10.5”). The HSE-NPL slide is manually centered to the objective on the bands 1-2. The focus is manually adjusted using the Z-knob.

The slide is scanned in the Z-direction and the same processing as the diagnostic app is used in order to obtain the best composite image from 44 slices interspaced at 0.5um in the z-direction. The images are kept in an internal xRapid QC database. Each image is further checked for quality and given a pass or fail score (binary).

### 6.4.2. Scale

The scale and gratings/grids displayed are displayed by software, and factory calibrated to standard traceable calibration slides (Ted Pella slides 2280-11, 2280-13, 2280-15).

The calibration factor for the images captures is 1415 pixels for 100µm. The maximum error permitted is ±5 pixels, that is approximately 0.35µm. The scale is checked for all microscopes on the app by simply imaging a square grid with a 50µm pitch and checking that the Walton Beckett graticule matches the spacing. In the image below the WB graticule is reasonably within 3 pixels of the grating limits.

![][27]

Figure 6.20. Application view of the 50µm square pitch graticule

The image captured using the same process as the diagnostic is checked for scale: the image is 1800 pixels in both width and height, and the dimensions determined are marked on the image below.

![][28]

Figure 6.21. image captured of a 50µm square pitch graticule

While the graticule dimensions should be checked on the measurement screen for quick validation, the only important piece of data is contained in the images captured — the measurement screen is a reflection of the scale determined from a captured image. The process is the following:

-   first, position the calibrated slide (grid or scale) conveniently on the microscope, and focus on the lines that need be measured;

-   Second, capture the image(s) by starting the test

-   Third, interrupt the test after a few steps — the microscope will have run out of grid area

-   Fourth, export the images to a PC/Mac by means of the usual way for iOS and your operating system.

-   Finally, measure the two orange lines shown in Figure 6.21. This should be around 1400 pixels for a space between consecutive ticks or lines of 100µm.

### 6.4.3. Precision/Accuracy versus Proficiency Testing

The xRapid Phase Contrast Microscope (PCM) has a built-in artificial intelligence (AI) and mechanical controls that work in tandem with an iPhone 7, iPhone 8, and iPad to drive filter analysis of airborne fibers per the NIOSH 7400 method, type A rules (other rules are available per chosen standard). The purpose of the evaluation is to thoroughly check and report on the performance of the product against the method set by NIOSH 7400 Recommendation and other performance standards from typical samples to proficiency test samples.

xRfiber has been evaluated versus proficiency test slides. The conditions were set to mimic real-world testing of airborne fibers collected on 0.80µm MCE filter media per the NIOSH 7400 Rev 1994 Method. This entailed a checklist to determine and document that the PCM is aligned, resolution calibrated, and field of view/graticule measured. In addition, per NIOSH requirements, blanks were incorporated into the testing regimen along with samples at low, medium, and high fiber loadings. The composition of these samples includes an amalgam of fiber deposition including chrysotile and/or amphibole asbestos and man-made fibers. Each sample was analyzed three times and the average evaluated against the known value/ranges. Fresh samples were prepared using the xRfiber template (cf. Appendix), and the starting position over the filter was varied between the three consecutive runs by approximately 500um.

Samples from proficiency test rounds over the last two years were used, the results are shown below.

![][29]

Figure 6.22: plot of the results of the three repetitions with various random start positions versus the reference count of proficiency samples. The empty boxes represent the lower and upper acceptable bounds, while the bullets are the measurement results, color coded per run. The Reference Value and acceptable bounds are determined from a number of laboratories not taking part in the proficiency round, which have been known to provide a reliable analysis. From the results of those laboratories, an average value is calculated (the Reference Value), together with a standard deviation. The acceptable range is within three standard deviations.

Based on these results, baring the natural deviations due to the randomness of the samples, one concludes that all results of quality control slides are in range.

### 6.4.4. Confidence values

The confidence values reported in the results are calculated using the equations given in NIOSH 7400, which describe the lower confidence limit (LCL) and higher confidence limit (HCL), as:

$$ LCL(n) = \frac{2n + 2.6^2-\sqrt{\left(2.6^2+2n \right)^2-4 \left(1-2.6^2 Sr^2 \right) n^2}}{2 \left(1-2.6^2 Sr^2 \right)} $$

where n is the number of fibers detected, and Sr is a “subjective inter-laboratory relative standard deviation, which is close to the total inter-laboratory Sr when approximately 100 fibers are counted”.

The latest revision of NIOSH 7400 states that “From these equations, the confidence limits accounting for both subjective microscopist and Poisson components for various fiber counts are calculated by taking Sr = 0.2. The intra- and inter- microscopist variability may be greater if quality control is poor”. Accordingly, xRfiber uses a value of Sr = 0.2, corresponding to a confidence interval of 0.95.

### 6.4.5. Results of Proficiency test rounds

The results obtained at some customer sites using xRfiber are reported in the three following tables. Should your results differ greatly from those, please contact [support@xrapid-group.com] .

Table 6.1: Results of IHPAT round 217

![A screenshot of a cell phone Description automatically generated]

Table 6.2: Results of IHPAT round 218

![A screenshot of a cell phone Description automatically generated][30]

Table 6.3: Results of IHPAT round 219

![A screenshot of a cell phone Description automatically generated][31]

6.5. Standard care and cleaning of the unit
---- 

### 6.5.1. Standard care

For optimal results, xRfiber must be used in a microscopy environment, that means:

-   Air regulated area to avoid dust.

<!-- -->

-   No vibration. The xRfiber platform must be installed in a stable and robust stage, uncoupled from floor vibrations.

Additionally, the microscope must be covered by its plastic pouch when not in use, to avoid the deposition of dust. Furthermore, the silicon tip must be inserted in the hole of the eyepiece of the trinocular when the iPhone/iPad is not on its cradle.

### 6.5.2. Cleaning the microscope

**WARNING**: Do not use detergents or aggressive liquids to clean the xRfiber microscope or its optics. A compressed air spray (not included) and the lens cleaning paper (included) are sufficient to perfectly clean the xRfiber platform.

Process for cleaning the xRfiber platform

1.  Remove the cradle

	1.  Begin by the socket head screws that they maintain the cradle support in the microscope head.

	2.  Remove the cradle with the eyepiece.

	3.  Loosen the three screws which maintain the eyepiece on the cradle cylinder and remove the eyepiece.

	4.  Clean the eyepiece using a dust air spray, clean it on its top and on its bottom.

	5.  If some impurities remain on the lens, use a lens cleaning paper (always with linear motion), and use the compressed air spray when finished.

2.  Remove the trinocular tube by loosening manually the two screws maintaining it

3.  Use the compressed air spray to clean the glass on the top of the head.

4.  Remove the head of the microscope using a 2.5mm Allen wrench.

	1.  Remove the Olympus objective from the turret.

	2.  Turn the turret to place the opened orifice in line with the optic train. From the top of the microscope, use the compressed air spray to clean the microscope and the turret.

5.  Reassemble the head of the microscope.

6.  Reassemble the trinocular tube.

7.  Place the eyepiece in the cradle cylinder and slowly fasten the 3 screws to maintain it.

8.  Reassemble the complete cradle and maintain it fastening both screws on the microscope head.

9.  Use the compressed air spray to clean the objective and reassemble it on the turret.

10. Use the compressed air to remove dust on:

-   The lenses on the top of the condenser.

<!-- -->

-   The glass on the top of the light diaphragm.

If use the front oculars are in use, to clean them:

-   Remove both oculars using a 1.5mm Allen wrench.

<!-- -->

-   Use the compressed air spray to clean inside the microscope head oculars orifices.

-   Use the compressed air spray to clean both oculars on their top and on their bottom. If some impurities are still existing, use the lens cleaning paper to remove them (every time with linear motion), and use the air compressed spray to finalize the oculars cleaning.

The xRfiber microscope is now normally clean to proceed with the analysis. Do not forget to clean your Apple device camera lens using the lens cleaning paper.

6.6. Updating the App
---- 

From time to time, the app may be updated from the App Store, over two ways:

-   in the background if this option was checked in the iOS App Store

<!-- -->

-   by checking if an update is present, if auto-updates are not allowed.

In all cases, xRapid will contact all customers before an update is released.

**NOTE**: an update of the app does **NOT** cause any loss of data.

**NOTE**: do **NOT** delete the app before updating it, this will cause a loss of data.

6.7. Troubleshooting

A list of most common issues is given in this section. In all cases, when in doubt contact support@xrapid-group.com.

*Issue: The light does not switch on*

*Resolution*:

-   Is your microscope currently plugged in a power source, and does your power source surely work (110V 60Hz, 230V 50Hz)?

<!-- -->

-   Is your microscope switched on?

-   Do you use the power supply delivered with microscope?

-   Try to switch off and switch on again your microscope, it could be in the sleeping mode.

*Issue: My Apple device does not charge when I plug it on the USB microscope socket*

*Resolution*:

-   Is the microscope light on?

<!-- -->

-   If yes, try with another lightning cable.

-   If no, please refer to ‘The light does not switch on’.

*Issue: No microscope found by the xRfiber App*

*Resolution*:

-   Kill the xRfiber App and switch off your microscope.

<!-- -->

-   Is your Apple device Bluetooth on?

-   Switch on your microscope.

-   Does the microscope light blink three times?

-   If no, please refer to ‘The light does not switch on’.

-   If yes, reopen the App, the microscope should become visible and connected in a few seconds.

*Issue: The microscope does not move when I launch a diagnosis*

*Resolution*:

-   Ensure that your Apple device is not connected with another microscope.

*Issue: The picture is dark on my Apple device display*

*Resolution*:

-   Ensure that the Apple device is in the correct place in its cradle and its camera is aligned with the cradle camera orifice.

<!-- -->

-   Ensure that the turret is turned well, the objective must be in line with the optics train.

-   Is the condenser diaphragm in its ‘PH’ position?

-   Is the microscope light on? If no, please refer to ‘The light does not switch on’.

*Issue: Shadow in a portion of the field of view*

*Resolution*:

-   Is the condenser on its uppermost position?

<!-- -->

-   Is the Apple device placed well in the cradle? Its camera must be aligned with the cradle orifice.

-   Is your cradle parallel with the stage? A level tool is available in the box to help you for the settings.

*Issue: Vibrations on images captured*

*Resolution*:

-   Ensure that your slide holder is tightened enough, if no, use both thumb screws to tighten it.

*Issue: The images contrast is not as good as usual*

*Resolution*:

Please refer to the user manual for light and PCM alignment setup.

For any other issue, please contact the xRapid support team at support@xrapid-group.com or by scanning the QR code placed under your microscope.

*Issue: the count on blank slides is high*

*Resolution*:

-   Check that the optics are clean, refer to the manual for cleaning them if this is not the case

-   Check that the slide is really blank: frequent cases of contamination on unsealed slides have been observed

-   Contact [support@xrapid-group.com] in case of doubt.

## 6.8. Limitations

The app is known to have some limitations when samples are damaged or have been poorly prepared. In particular, those cases:

-   undissolved filters

<!-- -->

-   overloaded filters

-   inconsistent filters

	-   damaged/broken filters

	<!-- -->

	-   unleveled filters

-   slides with too many bubbles entrapped

-   filters with fibers on both faces (cross contamination)

-   dirty slide coverslips and/or slide bottom surface

-   unknown objects, e.g. mold

will eventually lead to either a poor performance or erroneous results.

Let us now describe those in detail and see the potential resolutions.

### 6.8.1. Undissolved filters

#### Overview

When the acetone atomizer is not functioning properly, for instance not heating up to the required temperature of 70°C, the filter will be dissolved only partially. The issue, with xRFiber working on the luminance channel, are that:

-   the detection of gridlines is hampered,

<!-- -->

-   the sample appears to the AI as overloaded,

-   more generally the sample does not enable detection of fine chrysotile fibers.

As a result, the app performs poorly on those samples, and may not yield accurate results. When such a sample is detected, the app switches to a “safe” mode, which will not detect fine fibers but only consider coarse ones.

#### Resolution

The only solution is to prepare better samples, or to read those slides manually. To prepare better samples:

-   make sure that the “Ready” light present on most atomizers indicates that the heater body of the atomizer is at the correct temperature

<!-- -->

-   if this last point is correct and you are still seeing undissolved filters, check the atomizer (compare to another working atomizer). Replace the atomizer in case it is damaged

-   if the atomizer is not the culprit, it may be worth checking the filters: have you changed brand, or the lot is inconsistent?

### 6.8.2. Overloaded filters

#### Overview

Depending upon the standard followed, the field is considered overloaded if more than 1/6th to 1/4th of the Walton-Beckett graticule is filled by objects (debris and/or fibers). This may be the case with field samples that have been obtained for long sampling times in dirty environments. Because the field is overloaded, the human analyst may have issues determining a meaningful fiber count. The AI is facing the same issue, actually. In some rare cases, we have obtained proficiency slides which also appeared overloaded, though they needed to be measured in a forced analysis.

In all cases, overloaded samples will display an *Overloaded* characteristic in the *Tests Log*.

#### Resolution

There are two main ways to solve this issue.

First, if the sample is highly overloaded, one may want to go back to the site and sample again with lower exposure times. The regional standard should have an indication of the different sampling strategies one may employ.

Second, in case one cannot re-sample, there is an override in the xRFiber app that may be handy. In this case the app will run the analysis in a forced mode irrespective of the overload characteristic of the field. Because of the large number of objects to be classified by the AI the analysis will take a longer time, and because of the high contents the fine fibers may not be visible to the AI either. Consider also that this breaks many of the hypothesis covered by the standard: the Poisson distribution of fibers and/or debris is generally not true, for example. The app xRFiber will only start the analysis in forced overload mode with the user accepting a disclaimer that the app is being forced to run in a mode that is not compatible with the standard it follows.

### 6.8.3. Inconsistent filters

#### Overview

There are two main kinds of inconsistent filters encountered in practice:

-   broken filters: in this case xRFiber detects the edge of the broken filter and doesn’t account for it as a fiber. It will also keep the focus quite accurately. However, it will miss a few fields which will be counted as zeroes (blank fields).

<!-- -->

-   uneven filters: an uneven thickness is only likely to happen if we have some applied force during the mounting of the sample. In most cases, xRFiber will not be disturbed by this change of depth of the filter: xRFiber is able to compensate for up to 5 micrometers of change of depth in either direction from field to field.

#### Resolution

Avoid using tools or applying any pressure to the coverslip, as is discouraged by any standard procedure.

If there is substantial debris in the air during sampling the aggregation of the debris could cause the filter to tear under the pressure of the pump.

### 6.8.4. Bubbles

#### Overview

In some cases, one will find some bubbles of entrapped air that have been generated during the mounting of the filter. xRFiber normally deals with those fields in the same way a human analyst would: it does not measure the field and jumps to the next one. In some rare cases where a large amount of bubbles is present, xRFiber may run out of sample area to measure.

Note: a large number of non-measurable fields will increase drastically the test duration.

#### Resolution

The only resolution is to prepare valid samples. If a single analysis fails or runs out of the sample, it may be worth trying to restart the analysis from another starting location where xRFiber may encounter less bubbles.

Depending on the standard used, one should check the paths in previous section in order to make an educated guess as to where to start the analysis.

### 6.8.5. Both surfaces of filter exposed to fibers

#### Overview

Cross contamination of the filter is most likely caused by uncleaned slide or the mishandling of the filter during preparation, for example setting the filter down on a surface prior to mounting it

#### Resolution

Care should be taken when preparing samples to avoid cross-contamination.

In the case where the filter can cannot be mounted into another sample, one should monitor the execution of xRFiber.

### 6.8.6. Dirty slide and/or cover slip

#### Overview

Two issues may occur. First, there may be so much objects on the top and/or bottom of the slide that some halos are induced by the phase contrast, which may confuse the AI into recognizing fields as bubbles — in this case the loss of contrast hinders the accuracy of the detection. Second, the AI may choose to focus on those dirty surfaces instead of the filter.

#### Resolution

Use a wipe to clean off the dust from the top and bottom surfaces. Use a good brand of coverslips and slides. Our technical support may point you towards adequate consumables.

### 6.8.7. Unknown objects

#### Overview

The xRFiber AI has been conceived to classify accurately fibers and debris. While it also has the capability to classify correctly some fiber-like objects, it has not yet been expanded to cover all of the following types of objects:

-   molds

<!-- -->

-   pollens

-   hyphae.

In most cases the results will show that the Poisson distribution is not valid over the full slide. And of course, when objects are very similar in appearance to fibers, they may be wrongly qualified as fibers.

#### Resolution

We are working actively on a way to discriminate contaminated air samples. In the meantime, we recommend that the slide is checked manually when both Poisson distributions are invalid. We do also welcome anomalous images captured using xRfiber from our users: this is included, after proper vetting, into our database of images for training our AI, so that this anomaly is properly accounted for the next time it is encountered.

# 7.   CHECKLISTS

# 7.1.  Proficiency testing

1.  Installation and training complete

	a.  Unit installed

	b.  Training received

	c.  Environment evaluated

	i.  Vibration free platform

	ii. Consistent, indirect lighting

	iii. Power supplies connected

2.  Verification of proper size of magnified Walton Beckett graticule image (100μm diameter) by direct comparison on the screen

3.  Confirmation of ability to control and move stage with in-app manual controls

4.  Verification of HSE/NPL Test slide compliance - lines in series 5 visible, some of the lines in series 6 are visible but not all

5.  Preparation of testing samples (45) completed: fresh samples processed from archived filters of proficiency inter-comparison exercises

	a.  Using xRfiber Template for preparation (optional)

	b.  Proficiency program samples from within the last five years

	i.  Eight proficiency chrysotile samples

	ii. Seven proficiency amosite (amphibole) samples

	iii. Five proficiency man-made fiber samples

	iv. Two proficiency “Blank” samples

	v.  Three production “Overload” samples

	c.  Live samples

	i.  Six samples with low fibers count

	ii. Seven samples with medium fibers count

	iii. Seven samples with high fibers count

6.  Samples analyzed

7.  Data sheet completed.



1.  Starting a series of measurements

1.  microscope plugged to the power source

2.  switch on the microscope

3.  Did the microscope light source blink 3 times when it was switched on

4.  Is the light permanently on

5.  Is the 40✕ objective aligned with the optics train

6.  align the condenser with the light source

7.  open the light source diaphragm to produce a Köhler illumination

8.  check the condenser diaphragm is on its PH position

9.  check the objective and phase condenser rings are centered and aligned

10. check the iPhone/iPad connect to the microscope

11. Eventually switch the operator

12. Check that the standard selected in Settings is appropriate

13. check the app moves the microscope stage in 3 orthogonal directions using the Manual functions on screen

14. check the focus can be adjusted within 2-3 Z-graduations between the eyepiece and the iPhone

15. Verification of proper size of magnified Walton Beckett graticule image (100μm diameter) by direct comparison on screen

16. Verification of HSE/NPL Test slide compliance - lines in series 5 visible, lines in series 6 partially visible

17. Preferably use the xRfiber template for slide preparation

18. Locate the slide 2mm from the corner of the quarter disc (filter)

19. Eventually change the sample ID

20. Press the start button

21. Always check that the first sample in a series is being captured correctly: no loss of focus, field to field translations are appropriate (no sticking points between samples and out of plane)

22. Check that blanks are reporting low counts, appropriately

23. Pull samples marked for QC in the app, or others at the operator’s choice, and either check them by passing them through xRfiber from a different start position, or reading them manually

24. Additional samples are processed from point 17 onwards.

25. Periodically check that the rings are aligned.

# 8. REFERENCES

NIOSH7400: Asbestos and other fibers by PCM 7400, 2019. NIOSH Manual of Analytical Methods, Fifth edition. *This revision replaces Method 7400, issue 2 (dated 08/15/1994)*

OSHA id 160: Asbestos in Air [*link*]

NOSHC-3003: GUIDANCE NOTE ON THE MEMBRANE FILTER METHOD FOR ESTIMATING AIRBORNE ASBESTOS FIBRES

2ND Edition. 2005 [*link*]

IRSST 243-1: fiber count. Technical and scientific reports and notes, Analytical method 243-1. 1995. [*link*]

HSG248: Asbestos: The analysts’ guild for sampling, analysis and clearance procedures. 2005. ISBN 9780717628759. [*link*]

NF X43-269: Qualité de l'air - Air des lieux de travail - Prélèvement sur filtre à membrane pour la détermination de la concentration en nombre de fibres par les techniques de microscopie : MOCP, MEBA et META - Comptage par MOCP. 2017. [*link*]

NBN T 96-102: Workplace atmospheres - Determination of asbestos fibre concentration - Membrane filter method with optical phase contrast microscopy. 1999. [*link*]

Pang07: A new parameter to evaluate the quality of fiber count data of slides with relocatable fields. 2007. Journal of Occupational and Environmental Hygiene, 4: 129-144.

  []: media/image1.png{width="2.744792213473316in" height="1.0258311461067366in"}
  [1]: media/image2.tiff{width="2.759027777777778in" height="4.015384951881015in"}
  [2]: media/image4.tiff{width="4.5176071741032375in" height="6.464420384951881in"}
  [3]: media/image5.tiff{width="4.5176071741032375in" height="2.99375656167979in"}
  [4]: media/image6.tiff{width="2.361111111111111in" height="2.375in"}
  [5]: media/image7.tiff{width="1.3888888888888888in" height="1.8611111111111112in"}
  [6]: media/image8.tiff{width="3.0694444444444446in" height="1.8472222222222223in"}
  [7]: media/image9.tiff{width="2.2222222222222223in" height="1.6527777777777777in"}
  [8]: media/image10.tiff{width="2.2222222222222223in" height="1.6527777777777777in"}
  [9]: media/image11.tiff{width="1.4444444444444444in" height="1.4861111111111112in"}
  [10]: media/image12.tiff{width="1.4444444444444444in" height="1.4861111111111112in"}
  [11]: media/image13.tiff{width="1.4444444444444444in" height="1.4861111111111112in"}
  [12]: media/image14.tiff{width="1.5in" height="1.5in"}
  [13]: media/image15.tiff{width="1.5in" height="1.5in"}
  [14]: media/image16.tiff{width="1.5in" height="1.5in"}
  [15]: media/image17.tiff{width="1.5in" height="1.5in"}
  [16]: media/image18.png{width="4.5176071741032375in" height="3.766554024496938in"}
  [17]: media/image19.png{width="6.295833333333333in" height="3.5256944444444445in"}
  [18]: media/image20.png{width="6.295833333333333in" height="3.5256944444444445in"}
  [19]: media/image21.png{width="6.295833333333333in" height="3.588888888888889in"}
  [20]: media/image22.png{width="6.295833333333333in" height="3.2736111111111112in"}
  [21]: media/image23.png{width="6.295833333333333in" height="3.5256944444444445in"}
  [22]: media/image24.png{width="6.295833333333333in" height="2.7284722222222224in"}
  [23]: media/image25.png{width="6.295833333333333in" height="3.9520833333333334in"}
  [24]: media/image26.png{width="6.295833333333333in" height="2.7284722222222224in"}
  [25]: media/image27.png{width="2.7224267279090113in" height="3.62990157480315in"}
  [26]: media/image28.emf{width="4.5176071741032375in" height="4.687529527559055in"}
  [27]: media/image29.png{width="2.642836832895888in" height="3.7835181539807525in"}
  [28]: media/image30.emf{width="4.5176071741032375in" height="4.5176071741032375in"}
  [29]: media/image31.emf{width="4.5176071741032375in" height="2.661826334208224in"}
  [A screenshot of a cell phone Description automatically generated]: media/image32.png{width="6.3in" height="1.4949146981627297in"}
  [30]: media/image33.png{width="6.3in" height="1.4949146981627297in"}
  [31]: media/image34.png{width="6.3in" height="1.4949201662292213in"}

[1]:	mailto:%20support@xrapid-group.com

[image-1]:	https://github.com/xrapid-group/xrfiber/blob/master/Pictures/Figure_6_1.png