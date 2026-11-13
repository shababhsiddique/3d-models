# UnderShelfPoopDrawer — requirements

## From the user
- Two drawers hung under a shelf, side by side.
- Whole setup (shelf underside to drawer bottom) at most 3 in = 76.2 mm tall.
- Rail mount minimal; attaches to the underside of the shelf with 1/2 in or 3/4 in wood screws, easy to drive.
- One frame per drawer (two drawers on one mount would be about 270 mm wide, over the 256 mm bed).
- Printer: Bambu Lab P2S, build volume 256 × 256 × 256 mm. Every part must fit.
- Both drawers the same size; inner width 122 mm.
- Drawer length 240 mm, outside size.
- Integrated handle at the front bottom of the drawer, open underneath so it is easy to reach: fingers go up behind the front panel from below.
- Front panel covers the rails as far up as it can, with a little clearance to the shelf.
- No pull-out stop: the drawer slides fully out.

## Working decisions (change if the user says otherwise)
- Drawer hangs from runners along the top of its side walls; each runner rests on a 45° lip of the rail, so the drawer centres itself and both parts print without supports (drawer upright, frame upside down on its screw face).
- Drawer front panel is wider than the body and covers the rail ends; it is the closed stop.
- Screw holes for #6–#8 countersunk wood screws: 4.5 mm clearance, 90° countersink 9 mm, flush on the drawer side. Plate is 4 mm, so a 3/4 in screw goes about 15 mm into the shelf (shelf must be thicker than that); a 1/2 in screw about 8.7 mm.
- Six screws per frame, in three cross-bars (front, middle, back).
- Handle pocket roof: both long edges chamfered 5 mm at 45° (parameter roof_chamfer), so the printed bridge is 6 mm instead of 16 mm.
- Pocket housing, inside the drawer: top back edge chamfered 6 mm at 45° (user's "Chamfer 3") to save material; it runs parallel to the roof chamfer, leaving about 2.1 mm of wall between them. Its distance is the expression roof_chamfer + 1, so the wall stays when roof_chamfer changes.
- Clearances: 0.3 mm normal gap on the 45° slide faces, 0.5 mm side gaps, about 1.4 mm between drawer top and frame at rest; 1 mm between the two drawer fronts.
