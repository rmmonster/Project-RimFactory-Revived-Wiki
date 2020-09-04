# Developer Info and Tools

This page is for PRF crew and other modders to see behind the scene stuff.
We will list usefull info, comps and such in here, usefull when updating or making patches for PRF.

# Comps used in PRF:
### Theese are general and can be used on all type of def _(not thingclass specifics)_
**Help Tab**
```xml
<li><compClass>ProjectRimFactory.Common.CompPRFHelp</compClass></li>
```
Used to make Help button, it need a line in Language file called: `<DEFNAME_HelpText>Help text</DEFNAME_HelpText>`

**PRF lamps switch color comp.**
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
      </li>
```


## Assembler specific stuff
Assemblers in PRF are a general description linked to both smart assemblers and adaptive.
But also any preset assembler with locked recipes like Simple cooker

If its a preset assembler it needs to have this thingclass:
`<thingClass>ProjectRimFactory.SAL3.Things.Assemblers.Building_SimpleAssembler</thingClass>`
where the other 2 type have their own thingclass, but those are not used for other purposes.

For assemblers we have following Comps and mod extensions:
### Comps for assemblers
```xml
  <comps>
      <li Class="ProjectRimFactory.Common.CompProperties_PowerWorkSetting">        <!-- speed settings -->
        <speedSetting>true</speedSetting> <!-- use speed power boost or not? -->
        <minPowerForSpeed>0</minPowerForSpeed> <!-- power use for min setting -->
        <minSpeedFactor>1</minSpeedFactor> <!-- Slowest speed setting -->
        <maxPowerForSpeed>3000</maxPowerForSpeed> <!-- max power use -->
        <maxSpeedFactor>2</maxSpeedFactor> <!-- Max speed setting -->
        range settings
        <rangeSetting>true</rangeSetting> <!-- use range for input cells -->
        <minPowerForRange>0</minPowerForRange> <!-- power for minimum -->
        <minRange>1</minRange> <!-- Range on lowest setting (Radius) -->
        <maxPowerForRange>1000</maxPowerForRange> <!-- power for max -->
        <maxRange>3</maxRange> <!-- max range -->
        <rangeType>ProjectRimFactory.Common.RectRange</rangeType> <!-- not sure? think its shape of input cell -->
        <!-- range color settings, if not used just prf standards -->
        <blueprintMin>(1,1,1,1)</blueprintMin>
        <blueprintMax>(0.5,0.5,0.5,0.6)</blueprintMax>
        <instance>(1,1,1,1)</instance>
        <otherInstance>(1,1,1,0.35)</otherInstance>
      </li>
      <!-- this uses output cell on assemblers -->
      <li><compClass>ProjectRimFactory.Common.CompOutputAdjustable</compClass></li>

  </comps>
```
### Mod extensions for assemblers
```xml
  <modExtensions>
      <li Class="ProjectRimFactory.SAL3.Exposables.AssemblerDefModExtension">
        <importRecipesFrom>              <!-- import bills from a existing workbench, more then 1 can be used -->
          <li>ElectricStove</li>
        </importRecipesFrom>
        <workSpeedBaseFactor>2</workSpeedBaseFactor> <!--  Workspeed boost normal = 1 -->
        <skillLevel>20</skillLevel>      <!-- skill level set all skill to XX if not set skill = 10 -->
        <workingGraphicData>  <!-- Working texture swap -->
          <graphicClass>Graphic_Single</graphicClass>
          <texPath>SAL3/SpacerCookerWorking</texPath>
          <drawSize>(3,3)</drawSize>
        </workingGraphicData>
        <drawStatus>true</drawStatus>    <!-- Show working/idle status -->
        <doEffect>true</doEffect>        <!-- Sound and visual effect activate -->
        <overrideRecipeEffecter>         <!-- List of Recipe and Effecter to overwrite. -->

          <RecipeDef.defName Effecter="EffecterDef.defName" Sound="SoundDef.defName" />    <!-- Override a specific recipe effect and sound -->
          RecipeDef - see RimWorld\Data\Core\Defs\RecipeDefs\Recipes_*.xml                 <!-- find recipeDef here -->
          EffecterDef - see RimWorld\Data\Core\Defs\Effects\Effecter_*.xml                 <!-- find effectDef here -->
          SoundDef - see RimWorld\Data\Core\Defs\SoundDefs\*_Sustainers_*.xml              <!-- find soundDef here -->

        <CookMealSimple Effecter="Repair" />                                               <!-- example  -->
        <CookMealSimpleBulk Effecter="ButcherFlesh" Sound="Recipe_ButcherCorpseFlesh" />   <!-- example  -->
        </overrideRecipeEffecter>

        <defaultEffecter>Drill</defaultEffecter>        
       <!-- Effect that is used when RecipeDef.effectWorking and RecipeDef.soundWorking does not exist or is not defined in overrideRecipeEffecter.  -->
        <defaultSound></defaultSound>
      </li>
  </modExtensions> 
```