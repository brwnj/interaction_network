# Network Visualization using Cytoscape

Example of using Cytoscape to visualize gene interaction networks.

Given a gene interaction table where total mutations is found at a gene’s
intersection with itself and gene co-mutations in the remaining columns,
we parse into Cytoscape compatible, tab-delimited tables using Python. The
output from the script is imported into Cytoscape 3.0.2 generating the
interaction network.

In the saved Cytoscape session, we removed genes with fewer
than 5 total mutations bringing the count from 423 genes with 9317 interactions
down to 46 genes with only 596 interactions. Organizing the layout was done
using edge-weights based on co-mutation rates between genes. Node size
corresponds to a gene’s total mutations while node color corresponds to a nodes
relative centrality score. Genes in the center are colored red; the periphery
are green.

## Script Dependency

```pip install toolshed```
