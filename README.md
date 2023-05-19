# Find-all-pdf-in-sub-sub-folder

#This is a Bash script that allows the user to recursively search for PDF files in a specified parent folder and copy them to a destination folder.
#Here's how the script works:
#The user is prompted to enter the path of the parent folder where the script will start searching for PDF files.
#The script initializes a counter variable called pdf_count to keep track of the number of PDF files copied.
#There is a function called search_pdf_files that takes a folder path as an argument. This function is responsible for recursively searching for PDF files in the given folder and its subfolders.
#Inside the search_pdf_files function, a loop iterates over the contents of the current folder. If the current item is a directory, the function calls itself recursively to search for PDF files in that subfolder.
#If the current item is a file and its extension is .pdf, it is considered a PDF file. The script uses the cp command to copy the PDF file to the destination folder, which is set to /Users/user/Desktop/NEW in this example. The pdf_count variable is incremented by 1.
#After the function finishes executing, the script calls search_pdf_files initially with the user-provided parent folder path.
#Finally, the script prints a message indicating that the operation is complete and displays the total number of PDF files that were copied.
#Note: This script assumes that the destination folder (/Users/user/Desktop/NEW) already exists. If it doesn't exist, the script will fail to copy the files.
