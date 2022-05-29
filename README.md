# Absorbing Markovs

A little toy for visually constructing an absorbing markov chain/state machine that computes long-term absorbing probabilities and expected steps. An experiment with using native C++ code in Unity.

Try it out here: https://deynai.github.io/absorbing-markovs/

Usage Instructions:
- Create nodes with the New Node button
- Create transitions by clicking a nodes OUT socket and connecting it to an IN socket
- Enter a weight for transitions in the white box
- When finished constructing the graph, click Generate Matrix to compute long term behaviour (or some help messages for what went wrong)
- Select the appropriate starting state
- If changes are made after generating, click Generate Matrix again to refresh.

Note that all OUT transition weights must sum to 1, and a node with an OUT transition to itself with a weight of 1 is an absorbing state.

Controls:
- Drag node : Left Mouse Button
- Drag view : Middle Mouse Button
- Zoom in/out : Scroll wheel
- Remove selected nodes : Delete
- Remove connection : Right Mouse Button (on weight box)
