
# Scaling ETM scenarios to testing ground level

## Selecting the national reference scenario

There are two ways to specify the national reference scenario for the local testing ground:

1. Use an existing, saved scenario
2. Use a new scenario

Existing scenario's can be scaled directly. For a new scenario, the country and end-year must first be chosen.

## Scaling the national scenario to testing ground level

Before scaling the national scenario to testing ground level, you can specify the scaling variable. There are two options:

* the number of residences
* the number of residents

Once the scaling variable has been selected, you can enter a value for this variable. This determines how many residences – or residents – the testing ground will contain (see Figure 1 below).

![image](../images/Testing_ground.png)
> Figure 1. The scaling interface. Land, year-end and scaling can be chosen.

It is possible to explicitly exclude the following sectors from the testing ground

* Agriculture (excluded by default)
* Energy sector (included by default but with scaled down numbers)
* Industry (excluded by default)


Scaling of the national scenario to testing ground size happens as follows: all production and demand of energy is reduced by a fixed factor, which is the specified value for the scaling variable divided by the *original* value of the scaling variable.
If the national scenario, for instance, contains 10 million residences and your testing ground contains only 100 residences the scaling factor is given by:

	scaling factor = 100 / 10,000,000 = 0.00001.

All energy in the national scenario will be multiplied by 0.00001 to get the testing ground scenario. In addition to energy, the quantities of all technologies are scaled equivalently. For example, if the national scenario contains a million combi-boilers, using a scale factor of 0.00001 means there are only 10 combi-boilers left in the testing ground scenario.

Note: It may happen that scaling results in fractional numbers (e.g., 123.4 combi boilers.). In those cases, the number will be rounded to the closest integer. Exceptions to this rule are large power plants. It is possible to place 0.3 nuclear power plants in the testing ground.

## Excluding sectors from the testing ground

There are some sectors in the ETM that are less relevant for small-scale pilot projects:

* Industry
* Agriculture
* Energy (centralized production of electricity and heat)

You can exclude these from your testing ground by using the checkboxes in the scaling interface. This means that these sectors will have no energy demand or production, and are omitted from the interface.

However, if you choose to include these sectors in the testing ground scenario, their energy demand and production will be scaled with the scaling factor as described above.

## Adapting the testing ground scenario

The scaled scenario still has most of its properties equal to the national scenario that it originated from. The percentage of electric cars, or the number of solar panels is per household is still the same. You can now use the familiar professional interface of the ETM to update your testing ground scenario.

The interface for the testing ground scenario is identical to the [standard ETM interface](../general/Interface.md) with some modifications:

* The sectors excluded in the scaling step (optional) are removed from the interface
* The "other" sector (this is a statistical residual and irrelevant to the pilot)
* The section on storage (it will be replaced by more detailed calculations on testing ground level)
* The section on production of primary energy carriers is removed
* The section on network costs (it is replaced by the more detailed calculations on testing ground level)
* The section on fuel chain emissions is omitted


