
/*
* слово union означает объединение, либо-либо  type asd: number|string ; значит asd либо number либо string
* слово Intersections означает скрещивание, и-и type asd: IUser & TAsd; значит asd должен реализовать все типа полей IUser и TAsd
* */





In TypeScript, types are used to define the shape and behavior of values. Besides union types, TypeScript supports a
wide range of types, each serving a specific purpose. Here’s a comprehensive list of the main types available in
TypeScript:

1. Primitive Types
   These are the basic data types in TypeScript.

number: Represents numeric values.
string: Represents textual data.
boolean: Represents true or false values.
null: Represents an intentional absence of any object value.
undefined: Represents a variable that has been declared but not assigned a value.
symbol: Represents a unique and immutable value used as an identifier.
bigint: Represents whole numbers larger than the largest number number can represent.

2. Object Types
   These types represent non-primitive values.

Object: Represents any non-primitive type.
{}: Represents an object with no specific properties.
Interfaces and Classes: Define the shape of objects.

3. Array Types
   Array<T> or T[]: Represents an array of elements of type T.
4. Tuple Types
   [T1, T2, ...]: Represents an array with a fixed number of elements of specified types.
5. Function Types
   (param1: T1, param2: T2) => R: Represents a function taking parameters of types T1 and T2 and returning a value of
   type R.
6. Special Types
   any: Represents any type. Use with caution as it disables type checking.
   unknown: Represents any type but is safer than any because it requires type checking before use.
   void: Represents the absence of any type, usually used for functions that do not return a value.
   never: Represents the type of values that never occur, typically used for functions that never return (e.g., throw
   exceptions or have infinite loops).
7. Literal Types
   String literals: 'hello'
   Number literals: 42
   Boolean literals: true, false
8. Enum Types
   enum: Defines a set of named constant values.
9. Intersection Types
   A & B: Represents a value that is both of type A and B.
10. Conditional Types
    T extends U ? X : Y: Represents a type that is X if T extends U, otherwise it is Y.
11. Mapped Types
    { [P in K]: T }: Represents a type that maps properties P in K to type T.
12. Index Types
    keyof: Represents the keys of a type.
    T[K]: Represents the type of the property K of type T.
13. Utility Types
    TypeScript provides several utility types to facilitate common type transformations.

Partial<T>: Makes all properties in T optional.
Required<T>: Makes all properties in T required.
Readonly<T>: Makes all properties in T readonly.
Pick<T, K>: Picks a set of properties K from T.
Omit<T, K>: Omits a set of properties K from T.
Record<K, T>: Constructs a type with a set of properties K of type T.
Exclude<T, U>: Excludes from T those types that are assignable to U.
Extract<T, U>: Extracts from T those types that are assignable to U.
NonNullable<T>: Excludes null and undefined from T.
ReturnType<T>: Infers the return type of a function type T.
InstanceType<T>: Infers the instance type of a constructor function type T.
These types and constructs provide a powerful and flexible type system, enabling you to define and enforce the shapes
and behaviors of values in your TypeScript code.
