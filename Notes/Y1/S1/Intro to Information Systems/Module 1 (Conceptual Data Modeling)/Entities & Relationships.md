# ER (Entity Relationship Diagram)

ER Models provides a `graphical representation` of `data entities`
They are an easy way for clients to understand SQL Schemas

## Entities
An entity is essentially a physical or conceptual object which has
data associated with it

In the ER model:
• An entity type is represented as a rectangular box.
• Attribute names are represented by ovals attached to their entity type.
[Simple Entity][Notes/Y1/S1/Intro to Information Systems/Module 1 (Conceptual Data Modeling)/Simple Entity.png]

`key` constraint is a rule that an entity must have a distinct attribute that only that object can have to be associated to by

In an ER diagram the `key` attribute is underlined
Mutliple Keys are possible
 
Composite Attributes are attributes which can be made from smaller parts
Simple Attributes are attributes which have been simplified to a single part

A composite key is a combination of attributes to make up a key to an entity
They are written down with multiple underlines under multiple attributes

Multivalued Attributes are attributes which hold multiple values into one attribute
Multivalued Attributes are shown with double-lined ovals

Derived Attributes are attributes which can be derived from other attributes
e.g. age from birth_date

They are represented with a dotted line around them

Value sets specify the set of values that may be assigned to a particular
attribute of an entity
Value sets are not displayed on the ER diagram

`Entity Sets` is a collection of all entities of a particular entity type at any point of time

## Relationships

A `relationship` is an association among tow or more entities

A relationship type defines the relationship.
• In the ER model, relationships are represented using a diamond that
is connected to the associated entity types.
• A relationship type may have descriptive attributes.
• A relationship type may have key attributes

### Relationship Types
The degree of a relationship type is the
number of participating entity types
• 2 entities: Binary Relationship
• 3 entities: Ternary Relationship
• n entities: N-ary Relationship (3+ Entities)

Entity Roles:
Each entity in a relationship plays a `role`
The `role name` signifies the role of that participating entity

Recursive Relationships
Same entity types can participate more than once in the same
relationship type under different “roles”

Relationship Set
The collection of all relationships of a particular relationship type in the
database at any point in time is referred to as a relationship set

[Example][/Relationship Set.png]
