# How to Apply Input Masks in .NET MAUI Masked Entry (SfMaskedEntry)

The `Mask` property provides built-in support for applying input masks, allowing users to enter data in a predefined format.

To enforce structured data entry, set the required pattern using the `Mask` property:

* The `Mask` property defines the format that users must follow while entering data.
* The control automatically validates input against the specified mask and restricts invalid entries.

This approach helps ensure consistent data entry and improves the overall user experience by guiding users to enter information in the correct format.

### Benefits of Using Input Masks

* Enforces consistent input formatting.
* Reduces data-entry errors.
* Improves data accuracy and validation.
* Guides users during data entry.
* Simplifies the collection of structured information.

## Example Scenario

Consider a phone number field with the following mask:

**MainPage.xaml**

```
<ContentPage xmlns="http://schemas.microsoft.com/dotnet/2021/maui"
             xmlns:x="http://schemas.microsoft.com/winfx/2009/xaml"
             xmlns:editors="clr-namespace:Syncfusion.Maui.Inputs;assembly=Syncfusion.Maui.Inputs"
             x:Class="MaskedEntrySample.MainPage">
    <VerticalStackLayout>
        <editors:SfMaskedEntry x:Name="maskedEntry" 
                       WidthRequest="250"
                       ClearButtonVisibility="WhileEditing"
                       MaskType="Simple"
                       Mask="(000) 000-0000">
        </editors:SfMaskedEntry>
    </VerticalStackLayout>
</ContentPage>
```