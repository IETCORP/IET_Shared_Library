# IET Shared Library
## Styles
In App.axaml, add this line:
```xml
<Application.Styles>
	<StyleInclude Source="avares://IET_Shared_Library/Styles/TextStyles.axaml"/>
</Application.Styles>
```
Supported Tags should then automatically adjust Size & Font. You can use `Classes="Headline1"` inside a supported Tag to define the style.

**Tags supported**
- Button  
- TextBlock
- TextBox

**Classes supported**  
- Headline1 through 6  
- Subtitle1  
- Subtitle2  
- Body1  
- Body2  
- Caption  
- Overline  
- ButtonText  
- FloatingButtonText  
## Fonts
You shouldn’t need to reference Font files on their own, since the Text Styles use them. But if you want to use the fonts without the styles, you can do so by adding this line to App.axaml:
```xml
<Application.Resources>
	<ResourceDictionary>
		<FontFamily x:Key="Montserrat">avares://IET_Shared_Library/Assets/Fonts/Montserrat#Montserrat</FontFamily>
	</ResourceDictionary>
</Application.Resources>
```

## Window Icon
In any Avalonia .axaml file, within the Window tag, you can specify the Icon property like this:
```xml
<Window Icon="avares://IET_Shared_Library/Assets/Icons/iet-letters.ico"
```

## Window Icon
The folder “App Icons” can be used independently of IET_Shared_Library.dll. To set your project’s icon, copy-paste the icon you want into your project (usually in a sub-folder you can call “Assets”). Then, in the project’s Properties in Visual Studio, enter the file’s path.
