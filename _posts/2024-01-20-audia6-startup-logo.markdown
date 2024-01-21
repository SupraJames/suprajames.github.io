---
layout: post
title:  "Changing Startup Logo on Audi A6"
date:   2024-01-20 19:18:30 +0000
categories: vcds audi a6c7
---
OK, so this won't give you any extra horsepower, but it looks cool. The MMI and Instruments module in the Audi A6 (and probably other models) contains start up screens for the different sub models, i.e. A6, S6 or RS6. The logo which appears at start up is dependent on the coding (configuration) of that car when it left the factory.

With VCDS you can change the coding to display the logo of your choice.

### Using VCDS or any other tool to change your coding, or Adaptation values is **DANGEROUS**. If you make changes without full understanding, you can break your car. Don't do it!

TL;DR if you already know how to use VCDS

MMI Screen<br>
Control Module 5F - Information Electr.<br>
Long Coding, Byte 18<br>

Dashboard Display<br>
Control Module 17 - Instruments<br>
Long Coding, Byte 9<br>

![Dashboard](/assets/a6-startup-logo/dash.jpg)

![MMI](/assets/a6-startup-logo/mmi.jpg)

## MMI Screen

The following screenshots show the process to follow.

![Select Control Module](/assets/a6-startup-logo/pic0.png)

![Select Information Electr. Module](/assets/a6-startup-logo/iemod.png)

![Info Electric Module](/assets/a6-startup-logo/ie.png)

![IE Long Coding](/assets/a6-startup-logo/ie-lc.png)

Now comes the fun part. Use the Long Coding Helper to navigate to Byte 18. The drop-down menu will change, and show you the available options. Select the one you like, and close the window:

![IE Long Coding Helper](/assets/a6-startup-logo/ie-lch.png)

The new coding will be displayed. It is a very good idea to take a screenshot at this point, or record the coding so that it can be set back to default in case of problems:

![IE Long Coding Result](/assets/a6-startup-logo/ie-newcoding.png)

If you are happy, select Do It! and the new coding will be written to the module. Turn the ignition off and on again to see the new logo.

## Dashboard

The following screenshots show the process to follow.

![Select Control Module](/assets/a6-startup-logo/pic0.png)

![Select Instruments Module](/assets/a6-startup-logo/pic1.png)

![Instruments](/assets/a6-startup-logo/instruments.png)

![Instruments Long Coding](/assets/a6-startup-logo/instr-lc.png)

Now comes the fun part. Use the Long Coding Helper to navigate to Byte 9. The drop-down menu will change, and show you the available options. Select the one you like, and close the window:

![Instruments Long Coding](/assets/a6-startup-logo/insr-lch.png)

The new coding will be displayed. It is a very good idea to take a screenshot at this point, or record the coding so that it can be set back to default in case of problems:

![Instruments Long Coding](/assets/a6-startup-logo/instr-newcoding.png)

If you are happy, select Do It! and the new coding will be written to the module. Turn the ignition off and on again to see the new logo.


