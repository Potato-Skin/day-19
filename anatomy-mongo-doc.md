# Anatomy of a mongo document

```mongo
<!-- USER -->
   {
      _id: ObjectId("sdakjfgdsfjgkhsdfkgjhdsfkjghfsdkjlb"),
      name: "Gizem",
      lastName: "Wanka",
      working: true,
      studying: {
         class: ObjectId("asdkgjhsdfgkjdfhskgjhfdg")
      },
      friendsWith: ObjectId("another document inside same collection")
   }

   <!-- ANOTHER COLLECTION (classes) -->
   {
      _id: ObjectId("asdkgjhsdfgkjdfhskgjhfdg"),
      name: "Web Dev",
      partTime: true,
      students: [
        ObjectId("sdakjfgdsfjgkhsdfkgjhdsfkjghfsdkjlb")
      ]
   }
```

There ARE relations

CODE
X -> Mongoose (take care of mongo structure)
Mongo

## Types of relations

### One to One

User -> One DNA
(User holds the relation (key in the object) or the DNA holds it (or both))

### One to Many Relations

Restaurant -> Multiple recipes / Menus

### Many to Manu
User -> Friends -> Friends

Book -> Authors -> Books