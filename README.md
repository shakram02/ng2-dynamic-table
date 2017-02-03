# ng2-dynamic-table
A table for showing an array of items and some of their properties.

## What's special?
The special thing is that you use this table everywhere without needing to modify its code.
You just change the objects and properties you want to display in the component's attributes

### Example
assume an array which has some similiar object 
```TypeScript
    things: any = [
    {
      prop1: "hello",
      prop2: "asd",
      prop3: "asdasd"
    },
    {
      prop1: "hello1",
      prop2: "asd1",
      prop3: "asdasd1"
    }];
```
    
You want to display `prop1,prop3` you'll then use the component this way
```TypeScript
<app-dynamic-table [properties]='["prop1","prop3"]'></app-dynamic-table>
```

**Note that the argument is passed as a string array** Hopefully I'll find a better solution soon
