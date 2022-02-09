---
layout: beginning
title: How To Begin
description: Check for Image Corruption
light_mode: false
---

# How To Check If My Image Is Corrupt (Find MD5 Checksum)?

The md5sum is designed to verify data integrity using [MD5](https://en.wikipedia.org/wiki/MD5) (Message Digest Algorithm 5).

## Using Windows   
_by @kerrz_

1. Open Windows Powershell 
2. Go to the folder where your image file is present
3. In that folder, write: "Get-FileHash filename.img -Algorithm MD5"
4. Wait. This will take a lot of time. When finished, a number will show, which is the MD5 checksum.

Or you can find the MD5 checksum (and others) of your image file utilizing Hashtab [implbits](http://implbits.com/) - thanks to @share-and-enjoy. 

If the link above does not work, try this: [cnet](https://download.cnet.com/HashTab/3000-2094_4-84837.html)

When Hashtab is installed, you go to the image file in windows explorer, right click it >> Properties >> Hash tab. Depending on the size of the file and your computer, it will take some time to calculate the MD5 and SHA1. 

## Using Linux
_by @AzureOrange_

1. Open your favourite Terminal
2. Create a checksum of your image (This may take up to an hour, so grab a coffee):   
`# md5sum /PATH/to/file > checksum.md5 `
3. Check the integrety of that checksum (Another cup of coffee is recommended):   
`# md5sum -c checkmd5.md5 `
4. Compare the output hash with the provided one.

## Using Mac (Not yet tested)   
_by @AzureOrange_

1. Open your Terminal
2. Create a checksum of your image:   
` md5 -r /PATH/to/file `
3. Compare the output hash with the provided one.