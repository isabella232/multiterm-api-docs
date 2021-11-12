# TargetOnly property

## Name

Sdl.MultiTerm.TMO.Interop.Index.TargetOnly —          Flags whether the current index can be used only as target index.

## Type

Boolean
(read)

## Index Parameters
*none*

## Description


This property returns true if a particular index can be used only as target index, and not as source and target index.

You can use this property, for example, to exclude all target-only indexes from exclusion in a selection list.

## Sample


```cs
Sdl.MultiTerm.TMO.Interop.Indexes oIndexes;
oIndexes = myTermbase.Definition.Indexes;

//generate a list of indexes that can be source AND target
foreach(Sdl.MultiTerm.TMO.Interop.Index oIndex in oIndexes)
{
   	if(oIndex.TargetOnly==false)
      		Debug.WriteLine(oIndex.Label);
}
```
