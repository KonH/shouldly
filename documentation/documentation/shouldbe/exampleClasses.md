# Example Classes

The classes used in these samples are:

<!-- snippet: DocumentationExamples/ExampleClasses.cs -->
<a id='snippet-DocumentationExamples/ExampleClasses.cs'></a>
```cs
using System;

namespace Simpsons
{
    public abstract class Pet
    {
        public abstract string? Name { get; set; }

        public override string? ToString()
        {
            return Name;
        }
    }

    public class Cat : Pet
    {
        public override string? Name { get; set; }
    }

    public class Dog : Pet
    {
        public override string? Name { get; set; }
    }

    public class Person
    {
        public Person()
        {
        }

        public Person(string name)
        {
            Name = name ?? throw new ArgumentNullException(nameof(name));
        }

        public string? Name { get; set; }
        public int Salary { get; set; }


        public override string? ToString()
        {
            return Name;
        }
    }
}
```
<sup><a href='/src/DocumentationExamples/ExampleClasses.cs#L1-L45' title='File snippet `DocumentationExamples/ExampleClasses.cs` was extracted from'>snippet source</a> | <a href='#snippet-DocumentationExamples/ExampleClasses.cs' title='Navigate to start of snippet `DocumentationExamples/ExampleClasses.cs`'>anchor</a></sup>
<!-- endSnippet -->
