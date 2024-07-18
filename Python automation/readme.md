# Update file through Python automation

## Description
It was presented a scenario that as a security professional working at a
health care company one of the tasks is to update a file that identifies
employees who can have access to restricted data. I used the skills learned
during the course to automate this task using Python.  
The "allow_list.txt" file identifies the ip addresses allowed to access the 
restricted data. A separate remove list identifies IP addresses that should 
no longer have access to this content. 

## Summary
I created an algorithm that removes IP addresses identified in a remove_list 
variable from the "allow_list.txt" file of approved IP addresses. This 
algorithm involved opening the file, converting it to a string to be read, 
and then converting this string to a list stored in the variable ip_addresses. 
I then iterated through the IP addresses in remove_list. With each iteration, 
I evaluated if the element was part of the ip_addresses list. If it was, I 
applied the .remove() method to it to remove the element from ip_addresses.. 
After this, I used the .join() method to convert the ip_addresses back into 
a string so that I could write over the contents of the "allow_list.txt" file 
with the revised list of IP addresses.  
For the purposes of this exercise, I created a file_to_update.txt, so it was 
possible to compare the changes.



