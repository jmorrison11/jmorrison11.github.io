<!-- layout: page
title: "eshop"
permalink: /eshop/ -->

# Modifying the Microsoft eShop Program (eShoponWeb)
Using Microsoft Visual Studio 2019 I modified this program using a .NET structure in C#. I’ll list everything I did below:

- I Replace the items in the catalog with items from another vendor. I replaced the items with things from r the Saints Shop.
  - Modified the CatalogContextSeed class in the Infrastructure. Data folder. 
  - Modified the GetPreconfiguredItems() to define different, GetPreconfiguredCatalogBrands() to define different brands, 
  and GetPreconfiguredCatalogTypes() to define different types. 
  - Note that the first two integers in each item define the item type and brand.
- Added a new attribute: Color.
  - Added a new attribute to the CatalogItem class in ApplicationCore.Entities.
  - Modified the GetPreconfiguredItems() method in the CatalogContextSeed class in the Infrastructure.Data folder where it calls the CatalogItem() constructor.
  - Added the same attribute to the CatalogItemViewModel() in Web.ViewModels which is used to display the items.
  - Modified the GetCatalogItems() method in the CatalogViewModelService class in Web.Services so that the new attribute is copied from the CatalogItem into the CatalogItemViewModel. 
  In this GetCatalogItems() method, the code creates a new CatalogIndexViewModel and then copies each attribute over from the CatalogItem. 
  - Added a line to copy the new attribute over in the same way the name is copied over.
  - Modified the _product.cshtml in Web\Pages\Shared to display the new attribute. I added another line after the HTML that displays the item name, like <span>@Model.Color</span>
- Added an additional filter to the main page besides Brand and Type. This will required changing:
  - Web.Pages.Index.cshtml which has the HTML for the filters
  - Web.Services.ICatalogViewModelService which defines the interfaces to the filters
  - GetCatalogItems() in Web.Services.CachedCatalogViewModelService which is a cached decorator for
  - GetCatalogItems() in Web.Services.CatalogViewModelService
  - Added a new filtering class to ApplicationCore.Entities. This includes modifying CatalogFilterPaginatedSpecification and CatalogFilterSpecification.


##### [the repository](https://github.com/jmorrison11/eShopOnWebCore5_MorrisonJade)
###### [back to home](jmorrison11.github.io)
###### [back to project list](https://jmorrison11.github.io/projects)
