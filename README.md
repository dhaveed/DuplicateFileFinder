DuplicateFileFinder
===================

Duplicate File Finder Application developed in Java

Swing API was used for the GUI.

This application finds all duplicate files in a given directory.

The directory can be chosen using the 'Browse' button.

It uses a simple hash code for finding the duplicates. It is nothing but the filename + file size, which will be unique
for unique files and will be same for duplicate ones. Although it does not account for files which may have the same
name and the same file size but have different content, these are the corner cases and are not covered at this point
of time. Maybe a more advanced future version will have everything covered with a sophisticated hash function.

You are allowed to double click on the list of files to open any one of them. Direct deletion of the duplicate files or
any such feature has not been added yet.

The map used, maps the hash code to the list of file names associated with it (i.e. the duplicates)
        
        Map<String, List<String>> - key = hashcode
                                    value = linked list of duplicate file names
                                    
