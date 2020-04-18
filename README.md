## HighlightableTextBlock - Highlighting add-on for WPF TextBlock

### Quick Start
#### Installation:
Install-Package HighlightableTextBlock -Version 1.0.1.1
#### Modifying the XAML file

After installing HighlightableTextBlock:

* Open up the xaml file containing the TextBlock you wish to add highlighting. 
* Add this namespace reference to the XAML: 
  ```C#
  xmlns:hltb="clr-namespace:HighlightableTextBlock;assembly=HighlightableTextBlock"
  ```
  
* Locate the TextBlock declaration in the XAML. 
#### Template
```C#
  <TextBlock Text="{Binding SomeText}"
    hltb:HighlightableTextBlock.HightlightText="{Binding FindString}"
    hltb:HighlightableTextBlock.Italic="True"
    hltb:HighlightableTextBlock.HighlightBrush="Yellow" hltb:HighlightableTextBlock.HighlightTextBrush="Red"
    hltb:HighlightableTextBlock.Bold="True"/>
```
* Add this attribute:
```C#
  controls:HighlightableTextBlock.HightlightText="{Binding SearchText}" 
```  
* Ta-da! Now you have highlightable TextBlocks in your application!
* Customization:

  * Highlight color - controls:HighlightableTextBlock.HighlightBrush="Yellow" 
  * Highlight text color - controls:HighlightableTextBlock.HighlightTextBrush="Red"
  * Bold - controls:HighlightableTextBlock.Bold="True"
  * Italic - controls:HighlightableTextBlock.Italic="True"
  * Underline - controls:HighlightableTextBlock.Underline="True"
  
