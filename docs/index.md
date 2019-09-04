---
nav_order: 1
title: Home
---
# Example Docs
These examples demonstrate various aspects of the Symphony Allegro API. Each program is intended to show one
thing as clearly as possible with the minimum of clutter and in the clearest way possible. Each program 
is self contained and if you look at several examples you will see the same boiler plate code to deal with
command line processing and the like. This is intended to make each example readable on its own without
having to refer to utility classes or the super-class of the program to understand how it works.

```java

  /**
   * Set the _type attribute of the given mutable JSON object to the type ID of this type if it is null and
   * return an immutable copy.
   *
   * @param mutableJsonObject A mutable JSON Object.
   *
   * @return An immutable copy of the given object with the _type attribute set.
   */
  public static ImmutableJsonObject setType(MutableJsonObject mutableJsonObject)
  {
    if(mutableJsonObject.get(CanonRuntime.JSON_TYPE) == null)
      mutableJsonObject.addIfNotNull(CanonRuntime.JSON_TYPE, TYPE_ID);
    
    return mutableJsonObject.immutify();
  }
```

```
This is a snippet which is very wide. Now is the time for the quick brown fox to come to the aid of the lazy dog to aid the party of the mind broadening experiences which only lazy dogs and big frogs can begin to comprehend.
```