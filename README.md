# Snapmaker Community Tools Lbrary for Autodesk Fusion 360

This project is an effort to properly measure and classify the CNC bits available directly from [Snapmaker](snapmaker.com), specifically these two product listings: 

* [CNC Bits (3 Bits)](https://shop.snapmaker.com/products/cnc-bit?_pos=2&_sid=c19683085&_ss=r)
* [CNC Bits (5 Bits)](https://shop.snapmaker.com/products/cnc-bits-5-bits?_pos=1&_sid=c19683085&_ss=r)

In addition to validating the basic measurements and specifications such as number of flutes, this library for Fusion 360 will also take advantage of fields which are not populated in the official downloads on the vendor's webiste and github repo such as Vendor and especially **Product Id**.

As Snapmaker does not publish an actual Product ID on their website, we will use the letter "H" followed by an ordinal, with no special attempt to number the bits in any particular order. The Fusion 360 Tools Library has rich search and filtering capabilities, but sometimes you just want to quickly find the bit you decided to call "H2", because that's all the room you have to write on the back of the container with a sharpie.

# CONTRIBUTIONS

Are welcome. After importing this tools.json file into your copy of Fusion 360, make your edits in the GUI. (Or you can use a code editor of your choice.) Note that Fusion seems to create a .zip file called <library name>.tools upon export for some reason. You can rename/extract that to access the tools.json file. Be sure to check the following fields at a minimum:

* Vendor ("Snapmaker")
* Product Id - using an "H" followed by an unused integeter
* Product Link (look at store.snapmaker.com)
* Description - use the description on the website and package, using your judgement to be consistent. Do not include numbers as they are redundant with the other fields available.
* Diameter
* Shaft Diameter
* Overall Length
* Length below holder
* Shoulder length
* Flute length
* Coolant (set to "no" or "disabled", this will avoid useless errors when generating setups in Fusion)
* Type (e.g. "flat end mill")
* Number of flutes

If copying a tool from the OEM tools file, double check EVERYTHING. (I've seen a ton of issues, hence this repo!)

Mention in your log/PR the bits you are qdding, including Product Id, description, diameter, and shaft diameter.
