# 2026-11-23-FEA-nuance.md

## Big problems with little elements


11/23/2026 u-bolt simulation in prepomax
	Screenshots will be provided late

need ubolts for roof rack

so I went to McMaster-Carr; they have downloadable .STEP files for parts

I bring it into FreeCAD to Explode the Compound into it's individual parts
	(Main Body, Nut01/Nut02, and Mounting Plate)

Go through placing assembly constraints on parts, then export assembly file

I head on over to PrePoMax for FEA; start new document, import model, and start meshing parts

***This is where things get interesting (relatively speaking)

I mesh the Main Body, it goes fine, I mesh Nut01/Nut02, it goes fine

And then I try to mesh the Mounting Plate . . . 

It ran so long that I aborted the mesh algorithm

Figuring that it was between my assembly constraints I checked the distance joint of Plate/Nut01 & Plate/Nut02

Thinking that if there was a gap present between the Mounting Plate and the Nuts, even though I had set the distance joint to 0,
	this could be causing the elements to either stretch to fill the gap or be folded.

Looking at the terminal output, I did not see any issues with the Jacobian ratio but I did notice a glairing issue that
	I did not notice the first time . . . 

The element count it was trying to produce was orders of magnitude greater that what is normal for a 6.13" long part

So I go in to examine the geometry of the Mounting Plate to see what could be causing the need for so many elements

FILLETS!!!

Tiny fillets that are difficult to see (had to be a 1/32" although didn't measure) from a typical level of zoom

Thinking this is the actual problem, I go back into FreeCAD and try to remove these Fillets on the Mounting Plate

I cannot, no part history from McMaster; I try to just chamfer over them, no dice; I ended up making my own

Now with every thing set to how it should be, I have imported the new Ubolt to PrePoMax and that is where this journal entry's
	images are produced from

And the lesson's learned from this session will be recoded for reference later

