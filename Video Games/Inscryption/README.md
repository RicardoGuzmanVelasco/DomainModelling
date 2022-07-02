# Kalendra.Inscryption

Modelling Inscryption cards as C# POCOs from Unity Scriptable Objects.

## Domain modelling

### Entities
![](Images/DomainModel/DomainModel-Entities-CardTaxonomy.png)  
![](Images/DomainModel/DomainModel-Entities-Cards.png)  
![](Images/DomainModel/DomainModel-Entities-CardDetails.png)

#### Examples
![](Images/Cards/Squirrel.png)
![](Images/DomainModel/DomainModel-CardsExamples-Squirrel.png)

![](Images/Cards/Cat.png)
![](Images/DomainModel/DomainModel-CardsExamples-Cat.png)

![](Images/Cards/Rattler.png)
![](Images/DomainModel/DomainModel-CardsExamples-Rattler.png)

![](Images/Cards/Cockroach.png)
![](Images/DomainModel/DomainModel-CardsExamples-Cockroach.png)

## Analysis

### Entities

![](Images/Analysis/Analysis-Entities-Cards.png)

#### Invariants
![](Images/Analysis/Invariants/Invariants-Cards-ValueObjects.png)
![](Images/Analysis/Invariants/Invariants-Cards-Sigils.png)
![](Images/Analysis/Invariants/Invariants-Cards-CardModel.png)

## Design

### Infrastructure/Persistence
![](Images/Design/Infrastructure-CardsDefinition.png)

#### Examples
![](Images/Cards/ScriptObjs/Squirrel.png)
![](Images/Cards/ScriptObjs/Cat.png)
![](Images/Cards/ScriptObjs/Rattler.png)
![](Images/Cards/ScriptObjs/Cockroach.png)

This is just data definition. Sliders on stats don't call for any class invariant.  
It's only offering a handy way to design cards.  
> _However: while its min values are correct, max values of ranges are just dummy. Designers may require higher values to devs anytime, or even force lesser max values. This is Domain bussiness._  

For real class invariants, responsibility is in domain side — over entities whom these definitions are translated to.