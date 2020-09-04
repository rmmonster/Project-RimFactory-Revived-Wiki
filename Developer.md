# Developer Info and Tools

This page is for PRF crew and other modders to see behind the scene stuff.
We will list usefull info, comps and such in here, usefull when updating or making patches for PRF.

## Comps used in PRF:
`<li><compClass>ProjectRimFactory.Common.CompPRFHelp</compClass></li>`
Used to make Help button, it need a line in Language file called: `<DEFNAME_HelpText>Help text</DEFNAME_HelpText>`

PRF lamps switch color comp.
```xml      
      <li Class="ProjectRimFactory.Misc.CompProperties_Glower_ColorPick">
        <glowRadius>20</glowRadius> <!-- Glow radius like vanilla glow comp -->
        <glowColor>(252,199,139,0)</glowColor> <!-- Color when placed -->
        <key>PRF_Warm_White</key> <!-- Link to language file for translation use -->
        <moreColors> <!-- List extra colors with rgb code and language key/name -->
          <li><key>PRF_Cool_White</key><color>(140,200,250,0)</color></li>
          <li><key>PRF_Red</key><color>(217,80,80,0)</color></li>
          <li><key>PRF_Green</key><color>(80,217,80,0)</color></li>
          <li><key>PRF_Blue</key><color>(80,80,217,0)</color></li>
          <li><key>PRF_Cyan</key><color>(10,245,245,0)</color></li>
          <li><key>PRF_Yellow</key><color>(240,240,20,0)</color></li>
          <li><key>PRF_Magenta</key><color>(245,10,245,0)</color></li>
        </moreColors>
        <prerequisites> <!-- Required researche to unlock "button" -->
          <li>ColoredLights</li>
        </prerequisites>
      </li>```