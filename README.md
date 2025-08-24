# Siril used to register two photos of M13

On 2025-07-17, Mark Cunningham posted a success story about commissioning the
Orient Land Trust's very cool new 20" CDK20 telescope at Valley View Hot Springs:
 https://www.facebook.com/OrientLandTrust/posts/pfbid0g2YNfzykqQeNCvEQDLDnYKDo5HCoYkDHR3bSDbsNjikzh9vBdYATUgTEZCnyEA1sl

> Finally, I have all the calibration finalized on the new scope! Planewave CDK20 inch f7.77 Diffraction Limited! Here are two test shots taken with my Nikon D780 DSLR. Then a third photo taken with the ZWOAsi183mcpro CCD camera. Last photo is same object with the old Meade 16inch. M13 Globular Cluster is resolved to the CORE in the CDK20 as just a blob compared to the Meade telescope.

I took two of the included photos of M13 and uploaded them to https://nova.astrometry.net
to figure out exactly how they mapped to the sky ("plate fitting"). A little cropping
was needed so the text wouldn't confuse the algorithm.


```
https://nova.astrometry.net/user_images/13082523  Nikon D780 DSLR
https://nova.astrometry.net/user_images/13082520  ZWOAsi183mcpro CCD camera
```

Those pages also provide downloadable files in FITS format, which is suitable for applying
a wide variety of astronomical tools.

I then used the open-source program Siril to do a global star alignment to register the images,
rotating and scaling as needed so they would fit on top of each other.

First I had to rename the files and create a .seq file which specifies that they
are part of a sequence of shots.

```
m13vv01.fit  Nikon D780
m13vv02.fit  ZWOAsi183mcpro CCD camera
m13vv.seq    Simple text file describing the sequence
```

Siril produced corresponding files with a `r-` prefix.
Opening the frame list for the resulting sequence allows you to flip thru the images.

I also took screenshots, allowing anyone to flip back and forth between them for comparison.

```
m13-screenshot-01-commissioning.png
m13-screenshot-02-zwo.png
```
