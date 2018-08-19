# School in a Box
School in a box is an affordable, open source, all in one solution for managing the educational aspects
of a school from top to bottom. School in a box will keep track of students, teachers, and what classes
each are associated with. 

The purpose of School in a Box is to standardize the education platform and free the teachers from concerning
themselves with what to teach and dealing with tracking grades, and instead allowing them to focus on how to 
best teach their students while also providing quick and simple insight into grade metrics to find trouble areas
to focus upon.

As this application is open source, this README seeks to explain how School in a Box is built to allow an administrator
to quickly implement it, and if needed, modify the application to meet their needs.

## API Structure
The structure is meant to be as simple and logical as possible. How you would imagine a school being structured,
is how this API seeks to be structured. 

/\
/class\
/class/{id}\
/class/{id}/unit\
/class/{id}/unit/{id}/lesson/{id}/assignment\
/class/{id}/unit/{id}/lesson/{id}/assignment/{id}\

class: {\
&nbsp;&nbsp;&nbsp;&nbsp;id: int,\
&nbsp;&nbsp;&nbsp;&nbsp;subject: String(Enum/Lookup),\
&nbsp;&nbsp;&nbsp;&nbsp;gradeLevel: int,\
&nbsp;&nbsp;&nbsp;&nbsp;units: []\
}




