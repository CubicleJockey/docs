# Empty Constraint

`EmptyConstraint` tests that an object is an empty string, directory or collection.

## Constructor

```csharp
EmptyConstraint()
```

## Syntax

```csharp
Is.Empty
```

## Examples of Use

```csharp
Assert.That(aString, Is.Empty);
Assert.That(dirInfo, Is.Empty);
Assert.That(collection, Is.Empty);
```

## Notes

* **EmptyConstraint** creates and uses either an [EmptyStringConstraint](EmptyStringConstraint.md),
   [EmptyDirectoryConstraint](EmptyDirectoryConstraint.md) or [EmptyCollectionConstraint](EmptyCollectionConstraint.md) depending on the argument tested.
* A `DirectoryInfo` argument is required in order to test for an empty directory.
   To test whether a string represents a directory path, you must first construct
   a `DirectoryInfo`.
