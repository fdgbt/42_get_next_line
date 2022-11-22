# 42_get_next_line
Function to read each line of a file.  
Can be added to a static library.

## Man
Take a File Descriptor (const int) then a pointer to string (char **) as arguments.  
Return 0 (int) when file ended, 1 instead.  
Return -1 (int) if invalid argument or an error occured by OS limitation.

## Bonus
Manage various File Descriptor with internal chained list, allowing the reading of various files simultaneously without repositionning the read file offset.

## Notes
When file ended, internal function "ft_add_list" is called one last time to free the corresponding element of the chained list , avoiding memory leak.  
Internal structure is deliberately reduced to be compliant with the famous 42 Norm (V2).

## Keywords
Filedescriptors  
Bufferisation  
Parsing   
