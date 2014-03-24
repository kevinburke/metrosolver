# Mini Metro Solver

The goal of this repository is to figure out the optimal pattern for laying out
your [Mini Metro][metro] subway tracks.

 [metro]: http://dinopoloclub.com/minimetro/

### Steps

1. Use OCR to parse the positions of the stations and the existing subway cars,
and turn them into (x, y) coordinates.

2. Generate a list of all feasible combinations of subway routes.

3. Convert the subway routes into a min cost, min flow network.

4. Run the [out of kilter algorithm][ook] to determine which line is the best.

 [ook]: http://www.rand.org/content/dam/rand/pubs/research_memoranda/2008/RM5472.pdf

### Unanswered Questions

- What OCR software is best?

- How do we generate feasible subway routes?

- How do we make sure that the max flow only goes through one combination of
  subway lines?

- At what step do we incorporate the restriction on the number of tunnels?

- At what step do we incorporate the rule that subway lines cannot cross?
