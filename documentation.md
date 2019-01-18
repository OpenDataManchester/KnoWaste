# Draft Data Standard Documentation

**This documents is work in progress**

**Contributing Authors**: [Edafe Onerhime](https://ekoner.com/)

## About 

Words in **Bold** are important stakeholders, concepts or document for UK business waste. Phases and stages from the discovery documents are shown in 'single quotes'.

## Waste Management Scenarios

Waste management is the process of storing waste, transforming waste into a non-waste state (for example: recycling) or disposing of waste (for example: sending waste to landfill). 

When waste is managed, it can be:

* **Aggregated**: Waste in different containers with the same classificaion are added together
* **Co-mingled**: Waste in different containers with difference classifications are added together
* **Disposed**: Waste in a container is sent to a final destination, for example, landfill.
* **Separated**: Waste in a container is sorted and split, for example, a waste skip  of metal, rubble, soil and stones separated into skips of metal, rubble, soil and stones
* **Transformed**: Waste in a container is changed into non-waste, for example, glass from a bar is crushed into [glass cullet](https://en.wikipedia.org/wiki/Glass_recycling)

To simplify waste tracking, waste containers are issued a unique identifier, the **Waste Container ID** by the orignal **Waste Producer**. The **Waste Container ID** is shared with the **Consignee** along with the **Duty of Care Document**. A **Duty of Care Document** also gets a unique identifier, the **Duty of Care Document ID**. The **Duty of Care Document ID** tracks a non-hazardous waste job until a new **Duty of Care Document** is created. When this happens, a new **Duty of Care Document ID** is created and the old **Duty of Care Document ID** is added to the **Duty of Care Document** to create an audit trail.

The strategies below could help track waste in these waste management situations:

### Aggregated Waste

Waste in different containers with the same classificaion are added together. The new, aggregated waste containers are issued a new **Duty of Care Document** which means a new **Waste Container ID** for each new waste container and a new **Duty of Care Document ID**. The **Waste Holder** also stores the list of the previous **Waste Container ID** and **Duty of Care Document ID** that are part of this new waste job. 

### Co-mingled Waste

Waste from different sources with different **EWC Code** are added together. The new, aggregated waste is issued a new, unique **Waste Consignment Number**. The **Waste Holder** stores a list of all incoming **Waste Consignment Number** and **EWC Code** that are part of this new waste consignment. A new duty of care note is produced and the codes generated are passed along.

### Disposed Waste

Waste from the same source with the same **EWC Code** is sent to a final destination, for example, landfill. The **Waste Consignemnt Number** is retained and a final destination status or new **EWC Code** if necessary. A new duty of care note is produced and the existing code is passed along.

### Separated Waste

Waste from the same source with the same **EWC Code** is split. The new waste consignments are issued a new, unique **Waste Consignment Number** each and **EWC Code** if necessary. The **Waste Holder** stores the incoming **Waste Consignment Number** and **EWC Code** that were part of the originsl waste consignment. New duty of care notes are produced and the codes are passed along.

### Transformed Waste

Waste from the same source with the same **EWC Code** is changed. The new waste consignment is issued a new **EWC Code** if necessary and a code or description of the final product type. The **Waste Holder** stores the incoming **Waste Consignment Number** and **EWC Code** that were part of the originsl waste consignment. New duty of care notes are produced and the codes are passed along.

**Questions**
1. Do the journeys make sense?

## Non-Hazardous Waste

This section explains the phases business waste goes through from 'Aware' to 'Discovery' to 'Process' and 'Checking'. It is based on user research service blueprints from [Defra](https://www.gov.uk/government/organisations/department-for-environment-food-rural-affairs) and workshops with stakeholders including [Dsposal](https://dsposal.uk/).

### Aware

Awareness of waste classification and policy

![alt text][nhw_a]

[nhw_a]: https://github.com/OpenDataManchester/KnoWaste/blob/master/Data%20Flow_%20Non-Hazardous%20Waste_%20Aware.png "Data Flow: Non-Hazardous Waste: Aware"

'Aware' has 3 stages:

1. Assess - The **Waste Holder** asks: Is this waste? Is this controlled waste?
2. Classify - The **Waste Holder** asks: How do I classify the waste?
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
2. Does the **Waste Holder** (or any other stakehokder) need to know every time waste is re-classified?

### Discovery

Explore and understand what is required to be able to move waste

![alt text][nhw_d]

[nhw_d]: https://github.com/OpenDataManchester/KnoWaste/blob/master/Data%20Flow_%20Non-Hazardous%20Waste_%20Discovery.png "Data Flow: Non-Hazardous Waste: Discovery"

'Discovery' has 2 stages:

1. Assess - The **Waste Holder** asks: What do I need to do?
2. Select - The **Waste Holder** asks: Who can take my waste?

To continue tracking waste in 'Assess', we need to know:

1. what the **Waste Holder** needs to do and to track - not immediately clear from [Waste Duty of Care Code of Practice November 2018](https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/759083/waste-code-practice-2018.pdf) (England & Wales)

Next, the **Waste Holder** chooses a **Waste Processor**. To 'Select', we need to know:

1. Which public register was checked for the right **Waste Processor**
2. Where the waste is held - Once the waste is identified as **Controlled Waste**, it must be stored correctly according to the **Duty of Care Guidance** for the UK country where the waste is located. Guidance is available for different countries, so it's useful to know where the waste is held.
3. Who regulates waste at the location the waste is held - this could be useful later if we report to that regulator
4. Which local council is responsible for waste - the council may vary depending on the local policies or the type of waste
5. The selected **Waste Processor** who should be registered to act as a carrier, broker or dealer of waste
6. That the **Waste Processor** has a valid license to act as a carrier, broker or dealer of waste
7. That the **Waste Processor** has a registered exemption to accept such waste
8. That the **Waste Processor** has an environmental permit to accept such waste
9. When the **Waste Processor** was selected
10. When the **Waste Processor**'s registration, permits, licenses or exemptions were checked
11. The type of **Waste Processor**, for example a carrier, broker or dealer of waste

**Questions**
1. what the **Waste Holder** needs to do and to track when assessing a **Waste Processor**?
2. Does the **Waste Holder** need to track changes of selected **Waste Processor** for auditing or other purposes?
