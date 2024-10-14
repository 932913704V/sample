---
id: tutorial-Snipe-IT-Guide-Features
title: Features
---

<!-- ## Features -->

# Adding assets manually
Category, Manufacturer, Assets Model, and Suppliers are the main criteria required to add assets to the system.
1. **Create a category for the asset**.

    ![](../../../../../static/img/tutorial/category1.png)

Select the "**Categories**" from the dropdown list of settings located on the bar on the left side of the window. Then select "**Create New**" and fill in the details according to the asset category.

   ![](../../../../../static/img/tutorial/category2.png)

* Category Name - Name of the category
* Type - Select what types are used in this category. (Asset, Accessory, License, etc.)
* Category EULA - This field allows customizing your EULAs for specific types of assets.
* Use the primary default EULA instead. No primary default EULA is set. Please add one in Settings - You can add a default EULA from *Admin Settings > General Settings > Default EULA*
* Require users to confirm acceptance of assets in this category - *Yes* or *No*
* Send email to user on checkin/checkout - *Yes* or *No*
---
2. **Create custom fields if default fields are not sufficient**.

   ![](../../../../../static/img/tutorial/custom_field1.png)

Select the “**Custom Fields**” from the dropdown list of settings. First, create a new “**New Custom Field**” for the asset. Then create a “**New Fieldset**” and connect it with the newly created custom field.

   ![](../../../../../static/img/tutorial/custom_field2.png)

---
3. **Create the manufacturer of the asset/assets**.

   ![](../../../../../static/img/tutorial/manufacture1.png)

Select "**Manufacturers**" from the settings and then select "**Create New**" to onboard the manufacturer of the asset to the system. 

   ![](../../../../../static/img/tutorial/manufacture2.png)

---
4. **Create an asset model**.

   ![](../../../../../static/img/tutorial/model1.png)

Select "**Assets Models**" from the settings and then select "**Create New**" to a create new asset model.
* Asset Model Name - Name of the asset model
* Manufacturer - Select the manufacturer created at the ```step 3```.
* Category Name - Select the category create at ```step 1```.
* Depreciation - Create depreciation (*Settings > Depreciation*) and add it if your asset model has a depreciation.
* EOL - End-of-Life of the product.
* Fieldset - Select the fieldset created at the ```step 2```.
* Users may request this model - Users can request this asset from their accounts if this is selected.
* Image - Upload the asset model image to the system. Supported formats are jpg, webp, png, gif, and svg.

   ![](../../../../../static/img/tutorial/model2.png)

---
5. **Create the supplier of the asset/assets.**

   ![](../../../../../static/img/tutorial/supplier1.png)

Select “**Suppliers**” from the settings and then select “**Create New**” to add a new supplier to the system by filling in their details.

   ![](../../../../../static/img/tutorial/supplier2.png)

---
6. **Add the asset to the system.**

   ![](../../../../../static/img/tutorial/create_asset1.png)

Select "Create New" and then "Assets" from the top main bar to add an asset to the system.
* Company - Select the name of the company or division if you have more than one company or division onboarded. Otherwise, leave it empty.
* Asset Tag* - Tag of the asset. It must be unique. A mandatory field.
* Serial - Serial number of the asset. A mandatory field.
* Model* - Select the model created at the```step 4```. 
* Status* - There are four pre-configured statuses, and you can present the condition of the asset using them. You can check out the asset to the user, another asset, or location if you select the "Read to Deploy" option. A mandatory field.
* Asset Name - Name of the asset.
* Supplier - Select the supplier created at the```step 5```.
* Default Location - The default location of the asset belongs.
* Requestable - Users can request this asset from their accounts if this is selected.
* Upload Image - Photo of the asset. Better to update with the current condition of the asset.

  ![](../../../../../static/img/tutorial/create_asset2.png)
