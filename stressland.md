# Landscape stress maps

## Cookie Cutters × Stress Data



# Mapped stress data


## Land cover (grid)

 - Major break in classification pre/post 2000
 - Developed / bedrock confusion


## Point source

 - locations not trusted, office vs. outfall etc.
 - permitted vs. actual output
 - warm water vs. phenyl mercuric acetate


## Roads

 - Vector, sum length or convert to grid
 - Weight by type
 - Mapping inconsistent over time, road loss


## Population (census block)

 - Canadians census units can be very large


## Ag. census (counties)

 - Stocking levels, fertilizer purchase rates


## Soils (polygons)



# Cookie cutters


## Watersheds


## Interfluves


## Sub-Catchments



# Summary values


## Rich vs. minimal stress data

 - Rich stress data, dozens or hundreds variables
 - Minimal
   - % agriculture
   - % developed
   - population
   - road density
   - (point sources)
 - Easier to generate minimal set for trend analysis, 2000-2010
   changes.


## Principle component analysis

 - Incl. Ag. PC 1 etc.


## SumRel

 - Sum of all stressors, rescaled 0-1


## MaxRel

 - Maximum of all stressors, rescaled 0-1


## Euclidean Distance

$$ \sqrt{MaxRel(ag. vars)^2 + MaxRel(dev. vars)^2} $$



# Assigning stress to sites


## Area Weighting

 - Intersect site with watersheds, area weight by intersecting area


## Buffering

 - Used for embayments and high-energy shoreline
 - Get list of watersheds from buffer intersection
 - Area weight based on whole watersheds, not intersecting area



# Along shore agglomeration

 - For GLEI-2 “5971” or GLAHF 5593 watersheds, merge adjacent
   to address scale effects
 - Various algorithms
   - balance drained area
   - balance shoreline length



# Cookie cutters,<br/>the list


## GLEI-1

 - 762 “segment sheds”, US only, area draining to shoreline segment,
   segments run between midpoints between second order+ streams.
 - “Complexes”, area draining to GLEI-1 sampling areas, not synoptic.


## GLEI-2

 - Much of this work pre-dates GLEI-2
 - US and Canada
 - The “5971”, 5971 watersheds delineated by Tom Hollenhorst, US
   and Canada.
 - Embayments and High Energy sites, not synoptic


## GLAHF

 - 5593 watersheds, refinement of Tom's 5971, with input
   from Tom.
 - US and Canada, includes islands



# Mapped stress,<br/>the list


## GLEI-1

 - 200+ variables (Tom, again), soils, atmospheric deposition, etc.
   - PCA
 - also a subset, “CSI”, 86 variables
 - Land cover from an unpublished hybrid dataset by Pete Wolter


## GLEI-2

 - 4-5 variables (point source discontinued)
 - Land cover from an unpublished hybrid dataset by Pete Wolter


## “SOLEC-2017”

 - 4 variables, 2 times (2000 and 2010)
 - US and Canada
 - Land cover from published data



# Major pairings

 - GLEI-1 segment sheds × GLEI-1 200+ variables, PCA (US only)
 - GLEI-2 “5971” × GLEI-2 4 variables, SumRel, Euc. distance
 - SOLEC-2017 × GLAHF watersheds, Euc. distance
 - NRRI has a table of **26** different combinations of
   mapped stress and cookie cutters, and it's not complete.


