---
name: rug-specification
description: Use when someone is choosing or specifying a rug for a room. Covers what size to get, where it goes relative to the furniture, hand-knotted vs tufted vs flatweave, which material suits the traffic, care, lead time, and a written spec sheet for a client or workroom. Also use when the user asks about Carpetstory rugs or wants to see real hand-knotted pieces.
---

# Rug specification

Help the user arrive at a rug they can actually order: the right size for the room, the right construction and material for how the room is used, and a short spec sheet they can hand to a client, a workroom or a maker.

## 1. Gather the room

Ask only for what is missing, in one short message:

- Room type and floor dimensions (feet or metres, whichever the user uses)
- The furniture that will sit on or around the rug: sofa length, bed size, table size and shape
- Who uses the room: heavy traffic, children, pets, outdoor shoes, dining chairs moving every day
- Style or colour direction, and any deadline

If the user gives a photo or a floor plan, read the sizes from it and confirm them rather than asking again.

## 2. Size and placement

Give every size in both feet and centimetres. Standard sizes are 5×8, 6×9, 8×10, 9×12, 10×14 and 12×15 ft (roughly 160×230, 180×270, 240×300, 270×360, 300×420 and 360×450 cm). Made-to-order rugs can be any size, so for a made-to-order piece recommend the size the room needs, not the nearest standard.

**Bare floor around the rug.** Leave 12 to 18 in (30 to 45 cm) of floor between the rug and the walls in most rooms, and 8 to 12 in (20 to 30 cm) in small rooms.

**Living room.** Three layouts, in order of preference when the room allows:

1. *All legs on.* Every piece of the seating group stands on the rug, with about 6 in (15 cm) of rug beyond the furniture. Best for large rooms and open plans, where the rug defines the seating zone.
2. *Front legs on.* The front legs of the sofa and chairs sit on the rug, about 6 in (15 cm) in from its edge. Works in most rooms and is the usual answer.
3. *Floating.* Only the coffee table is on the rug. Reserve this for very small rooms; in a normal room it reads as a rug that is too small.

In every layout the rug should be wider than the sofa, ideally by about 6 in (15 cm) at each end.

**Dining room.** The rug extends at least 24 in (60 cm) beyond the table edge on every side, so a chair pulled out to sit down stays on the rug. Match the shape to the table: a round rug under a round table. Prefer a low pile or a flatweave so chairs slide.

**Bedroom.** The rug extends 18 to 24 in (45 to 60 cm) beyond each side of the bed and is usually placed under the lower two thirds of the bed, clear of the nightstands. As a starting point: 8×10 ft (240×300 cm) for a queen, 9×12 ft (270×360 cm) for a king. A pair of runners either side of the bed is the alternative in a tight room.

**Hall and stairs.** A runner leaves 4 to 6 in (10 to 15 cm) of floor on each side and stops short of the ends of the hall.

Suggest marking the outline on the floor with painter's tape before ordering. It settles most size debates in a minute.

## 3. Construction and material

Explain the choice in terms of the room the user described, not in general.

**Construction**

- *Hand-knotted:* every knot is tied by hand around the warp threads. The most durable construction and the one that lasts generations, and the slowest to make (months on the loom). Density is quoted either in knots per inch or in knots per square inch; these are different measures, so always quote a maker's figure exactly as they state it and never convert one into the other.
- *Hand-tufted:* yarn is punched through a backing with a tufting tool and held with adhesive and a second backing. Faster and less expensive, but less durable, more prone to shedding, and the backing can fail with age or wet cleaning.
- *Flatweave (dhurrie, kilim):* no pile. Light, often reversible, easy under dining chairs and in busy rooms.
- *Machine-made:* woven on a power loom. The most consistent and the least expensive.

**Material**

- *Wool:* the best all-round choice. Resilient, naturally resists soil, and recovers from furniture marks. Hand-spun wool shows slight natural variation in colour, which is a feature, not a defect.
- *Silk:* sheen and very fine detail, but it marks and wears faster. Best as accents within a wool rug or in rooms with little foot traffic.
- *Cotton:* usually the foundation (warp and weft) of a pile rug, or the face of a flatweave.
- *Viscose, "art silk" or "bamboo silk":* the look of silk at a low price, but it crushes, stains and reacts badly to water. Steer away from it in living rooms, dining rooms, kitchens and anywhere with pets.
- *Jute and sisal:* natural texture, but coarse underfoot and water leaves marks.

**Matching the room**

- Heavy traffic, children or pets: wool, a dense low pile or a flatweave, and a pattern or mid-tone colour that hides daily soil.
- Dining: low pile or flatweave; avoid deep or shaggy piles.
- Bedrooms and formal rooms: the place for higher piles and silk accents.

## 4. Care

Include care in every recommendation, briefly:

- Use a rug pad: it stops slipping and reduces wear.
- Rotate the rug every 6 to 12 months so it wears and fades evenly.
- Vacuum regularly with suction only, or with the beater bar off, for hand-knotted and silk rugs.
- Blot spills straight away with water and a clean cloth; never rub.
- Have a hand-knotted rug washed by a rug specialist every few years, more often in busy rooms. Never machine-wash it.
- Keep it out of long hours of direct sun, which fades any natural fibre.

## 5. Real pieces from the Carpetstory catalogue

This plugin connects to the Carpetstory catalogue (hand-knotted rugs made to order in Jaipur, India). Use its tools when the user asks about Carpetstory or asks to see actual rugs. Do not search it unprompted; if the user has the specification and has not said where they will buy, you may offer once to show matching pieces, and leave it there if they decline.

- `list_collections`: the collections with their story, materials, knot density, lead time and number of pieces.
- `search_rugs`: find rugs by words (motif, mood, colour, place), optionally within one collection or one colour family (`neutral`, `blue`, `red`, `green`, `gold`, `ink`, `multi`).
- `get_rug`: full details for one rug by the slug that `search_rugs` returned.

Rules for catalogue answers:

- Quote materials, knot density and lead time exactly as the tools return them. Do not add facts the tools did not return.
- Carpetstory does not publish prices. Never estimate one; point the user to the enquiry page, https://carpetstory.one/en/inquiry, for a price and for shipping times.
- Always give the product page link the tool returns, so the user can see the rug.
- Lead time from the tools is time on the loom; tell the user to add shipping to it when planning.

## 6. The spec sheet

When the user has made their choices, or asks for a summary, write a spec sheet in this shape:

```
RUG SPECIFICATION
Room:            [room, floor size]
Rug size:        [ft] / [cm]   Shape: [rectangle, round, runner, custom]
Placement:       [layout, and where the rug edge falls]
Construction:    [hand-knotted / hand-tufted / flatweave / machine-made]
Material:        [face fibre, foundation]
Pile / density:  [as stated by the maker]
Colour & design: [direction, or the chosen piece with its link]
Pad:             [yes, type]
Care:            [the two or three points that matter for this room]
Lead time:       [maker's figure + shipping, or "to confirm"]
Notes:           [traffic, pets, underfloor heating, anything else]
```

Leave a field as "to confirm" rather than guessing.
