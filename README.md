# Stock-driven extension of MISO2

This repository provides a stock-driven variant of MISO2 model. The MISO2 model (Material Inputs, Stocks, and Outputs) is a dynamic, inflow-driven material stock-flow model that covers 14 supply chain processes — from raw material extraction and processing, through stock-building and stock dynamics, to end-of-life flows and waste management. For detailed information, see the open-access publication: Wiedenhofer et al. (2024) and the [docs of associated repository](https://socialecologyboku.github.io/MISO2/).

In the stock-driven variant in this repository, the workflow has been reversed. Instead of starting from material inflows, the model begins with material stocks and derives associated flows. This enables the analysis of how future service provisioning and material requirements are shaped by existing and projected stocks. Through coupling with MISO2 energy and emission modules, energy consumption and GHG emissions associated with the production of materials can be assessed

**STACE: Stock-driven Austrian Circular Economy Model**

The newly developed STACE model (Stock-driven Austrian Circular Economy), which quantifies past, current, and future material stocks in Austria’s building, transport, and electricity sectors. 

STACE builds on the Excel-based CeAT model (Circular Economy Austria) developed by Haas et al. (2025), but enhances it by:

- Using updated inventory data from national statistics including Statistik Austria
- Integrating refined input data based on recently published scientific literature
- Embedding results into the stock-driven economy-wide MISO2 framework

The figure below illustrates the STACE–MISO2 model interface.

<img width="4106" height="2708" alt="System_Fig" src="https://github.com/user-attachments/assets/209f12e0-70fb-4c1e-bfbb-60215ff043df" />
Figure 1. Overview of the STACE and MISO2 model integration

**Key Features**

- Tracking of sectoral material stocks and flows in Austria from 2020–2100 with a focus on biophysical requirements of service provisioning (1)
- Sectoral coverage: Building, transport, and electricity sectors, with detailed distinctions such as: building types, heating systems, household appliances vehicles, road and railway types, and infrastructure, electricity production infrastructure
- Age-cohort-specific material stock data allowing for an improved calculation of material stock expansion requirements and outflows (2-3)
- Quantification of both operational (2e) and embodied (3e) energy consumption and GHG emissons
- Stock-driven perspective embedded in an economy-wide material stock-flow framework, allowing for the imapct of circular economy (CE) measures on overall resource use to be evaluated and for sustainable pathways to be identified (4)

The model is primarily developed for use in the ARCRP-funded HABITATION-CORRIDORS (Transforming essential provisioning systems through eco-social corridors) project: https://www.tuwien.at/ar/ifip/acrp-project-habitation-corridors

**Repository structure**

This repository builds on the main MISO2 model, which provides a code basis. The modified configuration file and data processing pipeline included here serve as the starting point for stock-driven applications.

**References**

Haas, W., Baumgart, A., Eisenmenger, N., Virág, D., Kalt, G., Sommer, M., Kratena, K., & Meyer, I. (2025). How decarbonization and the circular economy interact: Benefits and trade-offs in the case of the buildings, transport, and electricity sectors in Austria. Journal of Industrial Ecology, 29(2), 531–545. https://doi.org/10.1111/jiec.13619

Wiedenhofer, D., Streeck, J., Wieland, H., Grammer, B., Baumgart, A., Plank, B., Helbig, C., Pauliuk, S., Haberl, H., & Krausmann, F. (2024). From extraction to end-uses and waste management: Modeling economy-wide material cycles and stock dynamics around the world. Journal of Industrial Ecology, 28(6), 1464–1480. https://doi.org/10.1111/jiec.13575

**Authors**

The stock-driven MISO2 software as well as the STACE-MISO2 interface is currently being developed by:

- Benedikt Grammer
- Jan Streeck
- André Baumgart

**Contact**

For domain-related questions, please contact: andre.baumgart@boku.ac.at
For technical questions and bug reports, please open a GitHub issue or contact: benedikt.grammer@boku.ac.at









## Acknowledgments

This work was supported by the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (MAT_STOCKS, grant agreement No 741950), and the European Union's Horizon Europe programme (CircEUlar, grant agreement No 101056810). Funded by the European Union. Views and opinions expressed are however those of the author(s) only and do not necessarily reflect those of the European Union or granting authorities.
