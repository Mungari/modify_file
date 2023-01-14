# modify_file
This is a sample ansible role to modify a file. It requires the following variables:

| var_name | required | description            |
|----------|----------|------------------------|
| filename  | yes      | path to file to be modified (it has to be editable and has to exist, the role won't work otherwise) |
| line_to_change    |  yes  | what line to change. Has to be present in the file. Note: it will change the whole line unless replace_mode: true has been set |
| change | yes | what to change the line to |
| replace_mode | no | defaults to no |