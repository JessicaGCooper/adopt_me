``` 
return React.createElement("div", {}, [
    React.createElement("h1", {}, "Adopt Me!"),
    React.createElement(Pet, {
      name: "Teddy",
      animal: "Dog",
      breed: "German Shepherd",
    }),
    React.createElement(Pet, {
      name: "George",
      animal: "Bird",
      breed: "Cockatiel",
    }),
    React.createElement(Pet, {
      name: "Vashti",
      animal: "Cat",
      breed: "Calico",
    }),
  ]);
  ```

  The above code is javascript and the below code is the same translated into JSX

```
  return (
    <div>
      <h1 id='something important'>Adopt Me!</h1>
      <Pet name="Teddy" animal="Dog" breed="German Shepherd" />
      <Pet name="George" animal="Bird" breed="Cockatiel" />
      <Pet name="Vashti" animal="Cat" breed="Calico" />
    </div>
  );
```

# new section

```
return React.createElement    
("div", {}, [
  React.createElement("h1", {}, name),
  React.createElement("h2", {}, animal),
  React.createElement("h2", {}, breed),
]);
```

babel will translate the below code to the above code

```
  return (
    <div>
      <h1>{name}</h1>
      <h2>{animal}</h2>
      <h2>{breed}</h2>
    </div>
  )
```