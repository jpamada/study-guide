**Example 1**
This will return an error because there is no student with id of 3.
```js
function getStudent(id) {
  const students = [
    {id: 1, name: "Bob"},
    {id: 2, name: "Jeff"}
  ];
  
  const student = students.find(
    (student) => 
      student.id === id
  );
  
  if (!student) {
    throw new Error(
      "No student found";
    );
  }
  
  return student;
}

try {
  student = getStudent(3);
} catch (error) {
  console.error(error)
} finally {
  console.log("Log anyway")
}
```

___
[[03.01 Exception Types]]
