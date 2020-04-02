# Chainweb Client APIs

![Client APIs](client-apis.jpg)

# Chainweb with Per-Chain Consensus

*   Where are the new Blocks stored?
*   Why don't we store them per chain in PactService

![Chain Data in Pact Service](./overview-with-chaindb.jpg)

*   Braiding! Let mining take care of braiding?

![Braiding Validation Component](./overview-with-braiding.jpg)

Let miners pick the braiding and verify braiding for each block that arrives

![Chainweb without Cuts](chain2.png)

![Closeup of Chainweb without Cuts](chain2-closeup.png)

# Chainweb Consensus

*   *Consensus is on Chainweb level (not per chain)*

    In Code: `Web*` components (e.g. `WebBlockHeaderDb`)

*   Need algorithm that makes braiding validation efficient.

# Cut

![Chainweb with Consensus](./chainweb-with-consensus.jpg)

*   Inductively maintain a valid braiding

*   Distributed algorithm (Lattice, eventual consistency)



