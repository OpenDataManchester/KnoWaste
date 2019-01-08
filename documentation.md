# Draft Data Standard Documentation

**This documents is work in progress**

**Contributing Authors**: [Edafe Onerhime](https://ekoner.com/)

## About 

Words in **Bold** are important stakeholders, concepts or document for UK business waste. Phases and stages from the discovery documents are shown in 'single quotes'.

## Non-Hazardous Waste

This section explains the phases business waste goes through from 'Aware' to 'Discovery' to 'Process' and 'Checking'. It is based on user research service blueprints from [Defra](https://www.gov.uk/government/organisations/department-for-environment-food-rural-affairs) and workshops with stakeholders including [Dsposal](https://dsposal.uk/).

### Aware

Awareness of waste classification and policy

![alt text][nhw_a]

[nhw_a]: https://github.com/OpenDataManchester/KnoWaste/blob/master/Data%20Flow_%20Non-Hazardous%20Waste_%20Aware.png "Data Flow: Non-Hazardous Waste: Aware"

'Aware' has 3 stages:

1. Assess - The **Waste Holder** asks: Is this waste? Is this controlled waste?
2. Classify' - The **Waste Holder** asks: How do I classify the waste?
3. Re-classify - The **Waste Holder** has mis-classified waste or used an outdated (European Waste Catalogue) **[EWC Code](https://www.gov.uk/how-to-classify-different-types-of-waste)**

To begin tracking waste in 'Assess', we need to know:

1. Who the **Waste Holder** is (Also known as the **Holder of Waste** in Scotland) 
2. Where the waste is held - Once the waste is identified as **Controlled Waste**, it must be stored correctly according to the **Duty of Care Guidance** for the UK country where the waste is located. Guidance is available for different countries, so it's useful to know where the waste is held.
3. Who regulates waste at the location the waste is held - this could be useful later if we report to that regulator
4. Which local council is responsible for waste - the council may vary depending on the local policies or the type of waste
5. When the waste was accessed - this starts the clock on tracking

Next, the **Waste Holder** classifies the waste. To 'Classify', we need to know:

1. The **Waste Consignment Number** - A unique number that helps us track where waste ends up
2. When the waste was classified
3. The relevant **EWC Code**

If the **Waste Holder** makes a mistake, they can 'Re-classify'. We need to know:

1. When the waste was re-classified
2. The new **EWC Code**
3. Why the waste was re-classified. Some reasons include: Waste mis-classified, Outdated EWC used.

**Questions**
1. Should the **Waste Holder** be aware of weights and containers used for waste at this point?
2. Does the **Waste Holder** need to know every time waste was re-classified?

### Discovery

Explore and understand what is required to be able to move waste

![alt text][nhw_d]

[nhw_d]: https://github.com/OpenDataManchester/KnoWaste/blob/master/Data%20Flow_%20Non-Hazardous%20Waste_%20Discovery.png "Data Flow: Non-Hazardous Waste: Discovery"
